<template>
  <div id="navbar" class="flex h-[55px] w-full px-[4%] py-4 md:px-[5%]">
    <div class="flex justify-between">
      <li class="flex items-center">
        <RouterLink
          to="#"
          class="text-[30px] font-bold sm:text-[14px]"
          @click.native="scrollToTop"
        >
          Khen Veraque Doncillo
        </RouterLink>
      </li>
      <ul class="flex gap-5">
        <li class="grid h-full items-center">
          <RouterLink
            to="/"
            class="text-[15px] sm:text-[14px]"
            @click.native="scrollToTop"
          >
            Home
          </RouterLink>
        </li>
        <li class="grid h-full items-center">
          <RouterLink
            to="/about"
            class="text-[15px] sm:text-[14px]"
            @click.native="scrollToTop"
          >
            About
          </RouterLink>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
var prevScrollPos = window.pageYOffset;
window.addEventListener("scroll", function () {
  let currentScrollPos = window.pageYOffset;
  let navbar = document.getElementById("navbar");
  if (prevScrollPos > currentScrollPos) {
    navbar.style.top = "0px";
  } else {
    navbar.style.top = "-55px";
  }
  prevScrollPos = currentScrollPos;
});
function scrollToTop() {
  window.scrollTo(0, 0);
}
</script>

<style lang="scss" scoped>
#navbar {
  position: fixed;
  top: 0;
  width: 100%;
  color: #dad9d9;
  display: block;
  transition: top 0.5s;
  box-shadow: none;
  backdrop-filter: blur(10px);
  z-index: 99;
}

ul > li > a {
  display: block;
  color: #dad9d9;
  line-height: 2px;
  font-family: "Open Sans", sans-serif;
  font-weight: 700;
}

ul > li > a:hover {
  text-decoration: underline;
  transition: 0.3s;
}

ul > li > a:active,
ul > li > a:hover {
  outline: 0;
}
</style>
