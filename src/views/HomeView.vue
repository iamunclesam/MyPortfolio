<script>
import Hero from '@/components/Layout/hero.vue'
import Navbar from '@/components/Layout/navbar.vue'
import Loader from '@/components/Layout/pageLoader.vue';
import Skills from '@/components/mySkills.vue';
import SocialLife from '@/components/mySocialLife.vue';

export default {

  components: {
    Navbar, Hero, Loader, Skills, SocialLife
  },

  data() {
    return {
      isLoading: true, // Example: Set to true initially, update based on your application's loading state
    };
  },
}

</script>

<template>

  <!-- <Loader :isLoading="isLoading" /> -->

  <main>
    <Navbar />
    <Hero />


    <div class="about px-4 md:px-28 my-16">
      <div class="grid md:grid-cols-12">
        <div class="col-span-6 order-2 md:order-1 px-auto md:p-8">
          <div class="content">
            <div data-aos="fade-up" class="box mb-2 p-6 w-74 shadow-lg">
              <div class="flex justify-between h-auto items-center">
                <h1 class="text-purple-600 font-bold">Design</h1>
                <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24"
                  class="text-purple-600">
                  <path fill="currentColor"
                    d="M3 17.25V21h3.75L17.81 9.93l-3.75-3.75zm19.61 1.11l-4.25 4.25l-5.2-5.2l1.77-1.77l1 1l2.47-2.48l1.42 1.42L18.36 17l1.06 1l1.42-1.4zm-16-7.53L1.39 5.64l4.25-4.25L7.4 3.16L4.93 5.64L6 6.7l2.46-2.48l1.42 1.42l-1.42 1.41l1 1zM20.71 7c.39-.39.39-1 0-1.41l-2.34-2.3c-.37-.39-1.02-.39-1.41 0l-1.84 1.83l3.75 3.75z" />
                </svg>
              </div>
              <p class="text-gray-700 text-sm font-medium text-gray-500">Proeficient in modern asthethic designs</p>
            </div>



            <div data-aos="fade-up" class="box mb-2 p-6 w-74 shadow-lg">
              <div class="flex justify-between h-auto items-center">
                <h1 class="text-purple-600 font-bold">Front-end</h1>
                <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" class="text-purple-600"
                  viewBox="0 0 24 24">
                  <g fill="none">
                    <path d="M0 0h24v24H0z" />
                    <path fill="currentColor"
                      d="M14.62 2.662a1.5 1.5 0 0 1 1.04 1.85l-4.431 15.787a1.5 1.5 0 0 1-2.889-.81L12.771 3.7a1.5 1.5 0 0 1 1.85-1.039ZM7.56 6.697a1.5 1.5 0 0 1 0 2.12L4.38 12l3.182 3.182a1.5 1.5 0 1 1-2.122 2.121L1.197 13.06a1.5 1.5 0 0 1 0-2.12l4.242-4.243a1.5 1.5 0 0 1 2.122 0Zm8.88 2.12a1.5 1.5 0 1 1 2.12-2.12l4.243 4.242a1.5 1.5 0 0 1 0 2.121l-4.242 4.243a1.5 1.5 0 1 1-2.122-2.121L19.621 12z" />
                  </g>
                </svg>
              </div>
              <p class="text-gray-700 text-sm font-medium text-gray-500">Proeficient in responsive applications for
                better user experience.</p>
            </div>



            <div data-aos="fade-up" class="box p-6 w-74 shadow-lg">
              <div class="flex justify-between h-auto items-center">
                <h1 class="text-purple-600 font-bold">Back-end</h1>
                <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" class="text-purple-600"
                  viewBox="0 0 20 20">
                  <path id="oouiCode0" fill="currentColor"
                    d="M1 10.08V8.92h1.15c1.15 0 1.15 0 1.15-1.15V5a7.4 7.4 0 0 1 .09-1.3a2 2 0 0 1 .3-.7a1.84 1.84 0 0 1 .93-.68A6.4 6.4 0 0 1 6.74 2h1.18v1.15h-.86A1.32 1.32 0 0 0 6 3.62a1.7 1.7 0 0 0-.36 1.23V7a3.2 3.2 0 0 1-.28 1.72a2 2 0 0 1-1.26.77a2.15 2.15 0 0 1 1.26.79A3.26 3.26 0 0 1 5.62 12v3.15A1.67 1.67 0 0 0 6 16.37a1.31 1.31 0 0 0 1.08.47h.87V18H6.74a6.3 6.3 0 0 1-2.12-.29a1.82 1.82 0 0 1-.93-.71a1.9 1.9 0 0 1-.3-.72A7.5 7.5 0 0 1 3.31 15v-3.77c0-1.15 0-1.15-1.15-1.15zm18 0V8.92h-1.15c-1.15 0-1.15 0-1.15-1.15V5a7.4 7.4 0 0 0-.08-1.32a2 2 0 0 0-.3-.73a1.84 1.84 0 0 0-.93-.68A6.4 6.4 0 0 0 13.26 2h-1.18v1.15h.87a1.32 1.32 0 0 1 1.05.47a1.7 1.7 0 0 1 .36 1.23V7a3.2 3.2 0 0 0 .28 1.72a2 2 0 0 0 1.26.77a2.15 2.15 0 0 0-1.26.79a3.26 3.26 0 0 0-.26 1.72v3.15a1.67 1.67 0 0 1-.38 1.22a1.31 1.31 0 0 1-1.08.47h-.87V18h1.19a6.3 6.3 0 0 0 2.12-.29a1.82 1.82 0 0 0 .93-.68a1.9 1.9 0 0 0 .3-.72a7.5 7.5 0 0 0 .1-1.31v-3.77c0-1.15 0-1.15 1.15-1.15z" />
                  <use href="#oouiCode0" transform="matrix(-1 0 0 1 20 0)" />
                </svg>
              </div>
              <p class="text-gray-700 text-sm font-medium text-gray-500">Proeficient in backend technologies around
                NodeJs.</p>
            </div>
          </div>
        </div>

        <div data-aos="fade-left" class="col-span-6 order-1 md:order-2">
          <div class="content md:p-16 md:pt-0 pb-8">
            <code class="text-purple-500 text-sm "> About Samuel </code>
            <h1 class="text-6xl font-semibold text-white">Who am i?</h1>
            <p class="text-gray-500 py-4 text-sm">I am a web developer specializing in React and Node.js, with over 3
              years of experience in software development. I excel in creating robust and scalable web applications that
              enhance user experiences. Passionate about leveraging emerging technologies to drive innovation in the
              industry, I am committed to staying at the forefront of web development trends and best practices.</p>

            <p class="text-gray-500  text-sm">Innovation drives me. Let's connect to create impactful web experiences
              that shape the future.</p>

            <a href="#"
              class="inline-flex items-center justify-center py-3 mr-3 text-base font-medium text-center text-purple-500 rounded-lg bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900">
              let's connect
              <svg class="w-5 h-5 ml-2 -mr-1" fill="currentColor" viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd"
                  d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                  clip-rule="evenodd"></path>
              </svg>
            </a>
          </div>
        </div>
      </div>
    </div>

    <div class="projects md:px-28 px-4 my-10">
      <h1
        class="text-center h-20 text-5xl font-semibold bg-gradient-to-r from-purple-700 to-pink-800 bg-clip-text text-transparent ">
        My Projects</h1>
      <div class="grid md:grid-cols-12 my-16 mt-8">
        <div data-aos="fade-up" class="col-span-6 px-4 overflow-hidden">
          <div class="content">

            <a href="#"
              class="block max-w-full p-6 bg-gradient-to-r from-purple-700 to-pink-800 rounded shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">

              <h5 class="mb-2 text-2xl font-bold tracking-tight text-white dark:text-white">Aura Hospital Management System</h5>
              <p class="font-normal  text-gray-300 dark:text-gray-400">Aura HMS is a web software for an hospital that manages the day to day activities of the hospital. It was build with Vue.Js, NodeJs and Express server.</p>
            </a>

          </div>
        </div>

        <div data-aos="fade-up" class="col-span-6 px-4 mt-10 md:mt-0 overflow-hidden">
          <div class="content">
            <a href="#"
              class="block max-w-full p-6 bg-gradient-to-r from-purple-700 to-pink-800 rounded shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">

              <h5 class="mb-2 text-2xl font-bold tracking-tight text-white dark:text-white">The MovieFusion Movie App</h5>
              <p class="font-normal text-gray-300 dark:text-gray-400">Moviefusion is a movie web application built with Vue.js and Firebase technologies. It has features like collections, movie cast, watch providers and youtube trailers.</p>
            </a>

          </div>
        </div>

        <div data-aos="fade-up" class="col-span-6 px-4 mt-10 overflow-hidden">
          <div class="content">
            <a href="#"
              class="block max-w-full p-6 bg-gradient-to-r from-purple-700 to-pink-800 rounded shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">

              <h5 class="mb-2 text-2xl font-bold tracking-tight text-white dark:text-white">ShoppersNg Ecommerce App</h5>
              <p class="font-normal text-gray-300 dark:text-gray-400">ShopppersNg is an Ecommerce web application built with VueJs and fakestore api. It has store and add to cart feature.</p>
            </a>

          </div>
        </div>

        <div class="col-span-6 px-4 md:relative mt-10 md:mt-0 overflow-hidden">
          <div class="content md:absolute bottom-20 right-20">
            <div class="text-purple-600 text-md font-light underline">VIEW ALL PROJECTS</div>
            <p class="text-gray-500 pt-8 text-sm font-medium">Take a visit to my github repo</p>
          </div>
        </div>


      </div>
    </div>
    <!-- 
    <div class="my-skills py-20">
      <Skills />
    </div>


    <div class="socials my-20">
      <SocialLife />
    </div> -->


  </main>

</template>


<style>
.box {
  background-color: #0d0c0c;
}

.glow-neon-button {
  position: relative;
}

.glow-neon-button::after {
  content: '';
  position: absolute;
  top: -2px;
  /* Adjust as needed */
  left: -2px;
  /* Adjust as needed */
  right: -2px;
  /* Adjust as needed */
  bottom: -2px;
  /* Adjust as needed */
  z-index: -1;
  border-radius: inherit;
  background: linear-gradient(135deg, #147650, #147650);
  box-shadow: 0 0 10px #147650, 0 0 20px #147650, 0 0 30px #147650, 0 0 40px #147650;
  animation: glow-neon-animation 1.5s ease-in-out infinite alternate;
}

@keyframes glow-neon-animation {
  from {
    opacity: 1;
  }

  to {
    opacity: 0;
  }
}
</style>
