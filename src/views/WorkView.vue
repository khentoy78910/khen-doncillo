<template>
  <div class="mb-[25px] h-auto w-full px-[20.5%] lg:px-[10%] md:px-[5%]">
    <div class="intro mt-[120px] h-auto md:mt-[80px]">

      <div class="h-auto w-[100%] sm:hidden">
          <img
            src="../assets/imgs/Photo.jpg"
            alt="Image not found"
            class="h-auto w-[100%] rounded-md md:w-[90%]"
          />
        </div>

      <h1
        class="text-block-for-intro w-full text-[22px] leading-[50px] md:text-[18px] md:leading-[40px] sm:leading-[30px]"
      >
        Greetings! I'm a
        <span class="font-bold text-[#416bd8]">Third Year College Student</span>
            , a diligent working student currently 
            attending Cordova Public College. Alongside my academic pursuits, 
            I have a fervent passion for travel, which fuels my desire to 
            explore new destinations whenever I can. As I navigate through 
            my studies and work commitments, I also find solace in indulging 
            in various hobbies and interests.
            professional commitments. 
      </h1>
      <h3
        class="text-block-for-intro02 mt-[20px] md:mt-[10px] md:text-[16px] sm:text-[14px]"
      >
        Bachelor of Science in Information Technology
        <a href="https://www.facebook.com/cpcofficial2005" target="_blank">
          <span class="cursor-pointer font-bold text-[#416bd8]">
            Cordova Public College
          </span>
        </a>
      </h3>
      <div class="mt-[50px] flex items-center gap-4 md:mt-[30px]">
        <a href="https://www.facebook.com/khen.doncillo.7" target="_blank">
          <img
            src="https://www.svgrepo.com/show/503338/facebook.svg"
            alt=""
            class="w-[25px] md:w-[20px]"
          />
        </a>
        <a href="https://www.instagram.com/khendoncillo/" target="_blank">
          <img
            src="https://www.svgrepo.com/show/521711/instagram.svg"
            alt=""
            class="w-[25px] md:w-[20px]"
          />
        </a>
        <a href="https://github.com/lydenchai" target="_blank">
          <img
            src="https://www.svgrepo.com/show/512317/github-142.svg"
            alt=""
            class="w-[25px] md:w-[20px]"
          />
        </a>
      </div>
    </div>
    <div class="projects">
      <!-- <div
        class="mt-[50px] h-auto w-full md:mt-[30px]"
        v-for="project in projects"
        :key="project"
      >
        <Project :project="project" />
      </div>
      <div class="mt-[50px] h-auto w-full md:mt-[30px]">
        <h1
          class="other-project-title mb-[25px] text-[24px] md:mb-[15px] md:text-[20px] sm:text-[18px]"
        >
          Other Projects
        </h1>
        <div
          class="mb-[50px] h-auto w-full md:mt-[15px]"
          v-for="project in otherProjects"
          :key="project"
        >
          <Project :project="project" />
        </div>
      </div> -->
    </div>
    <div class="footer h-auto w-full">
      <Footer />
    </div>
  </div>
</template>

<script setup lang="ts">
// import Project from "../components/Project.vue";
import Footer from "../components/Footer.vue";

// const projects: any[] = [
//   {
//     name: "Rental Management System",
//     description:
//       "Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab, fugit eaque.",
//     details: {
//       title:
//         "lorem ipsum dolor sit amet consectetur adipisicing elit. Ab, fugit eaque.",
//       description: "description",
//     },
//     image: "https://bontub.com/bg-hero.png",
//   },
//   {
//     name: "KAS-PORTAL",
//     description:
//       "Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab, fugit eaque.",
//     details: {
//       title: "",
//       description: "",
//     },
//     image: "",
//   },
//   {
//     name: "Travona Hotel Room",
//     description:
//       "Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab, fugit eaque.",
//     details: {
//       title: "",
//       description: "",
//     },
//     image: "",
//   },
//   {
//     name: "Travona mini app",
//     description:
//       "Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab, fugit eaque.",
//     details: {
//       title: "",
//       description: "",
//     },
//     image: "",
//   },
// ];
// const otherProjects: any[] = [
//   {
//     name: "Sabay News Clone",
//     description:
//       "Lorem ipsum dolor sit amet consectetur adipisicing elit. Ab, fugit eaque.",
//     details: {
//       title: "",
//       description: "",
//     },
//     image: "",
//   },
// ];
</script>

<style lang="scss" scoped>

.text-block-for-intro {
  max-width: 100%;
  font-family: "Lato", sans-serif;
  color: #ebe6e6;
  font-weight: 900;
  letter-spacing: 0.3px;
}

.text-block-for-intro02 {
  margin-bottom: 0vh;
  line-height: 20px;
  color: #ebe6e6;
}

.footer {
  margin-bottom: 0vh;
  line-height: 20px;
  color: #ebe6e6;
}

// .other-project-title {
//   font-family: Lato, sans-serif;
//   color: #ebe6e6;
//   line-height: 55px;
//   font-weight: 700;
//   letter-spacing: 0.3px;
// }
</style>
