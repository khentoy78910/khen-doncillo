<template>
  <div class="w-full text-[#444444]">
    <div class="flex h-[100vh] w-full items-center justify-between md:h-[55vh]">
      <div
        class="flex w-full px-[20.5%] lg:px-[10%] md:mb-[50px] md:mt-[55px] md:px-[5%] sm:mt-[80px] sm:flex-col"
      >
        <div class="h-auto w-[100%] sm:hidden">
          <img
            src="../assets/imgs/Photo.jpg"
            alt="Image not found"
            class="h-auto w-[80%] rounded-md md:w-[90%]"
          />
        </div>
        <div class="w-[60%] sm:w-[100%]">
          <p class="text-[#fff] letter-spacing-[0.3px] tracking-wide md:text-[15px] text-[20px]">
            Hello there! My name is
            <span class="font-bold text-[#fff] text-[22px]">Khen Veraque Doncillo</span>, a
            passionate third-year college student with practical experience spanning 
            nearly three years, I possess strong expertise in HTML5, CSS3, and 
            JavaScript. My focus lies in developing aesthetically pleasing and 
            intuitive web applications that prioritize user experience. 
            I have honed my skills in Angular and Vue.js, relishing the opportunity 
            to translate design concepts into polished interfaces seamlessly.
          </p>
        </div>
        
      </div>
      
    </div>
    <div class="footer h-auto w-full">
      <Footer />
    </div>
  </div>
  
</template>

<script setup lang="ts">

import Footer from "../components/Footer.vue";

</script>

<style lang="scss" scoped>
.footer {
  margin-bottom: 0vh;
  line-height: 20px;
  color: #ebe6e6;
}
</style>
