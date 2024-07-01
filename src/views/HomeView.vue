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

            <div
              class="block max-w-full p-6 bg-gradient-to-r from-purple-700 to-pink-800 rounded shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">

              <div class="">
                <svg class="text-gray-200" xmlns="http://www.w3.org/2000/svg" width="3em" height="3em"
                  viewBox="0 0 2048 2048">
                  <path fill="currentColor"
                    d="M896 768v256H640v256h256v256h256v-256h256v-256h-256V768zm384 128h256v512h-256v256H768v-256H512V896h256V640h512zm576-512q40 0 75 15t61 41t41 61t15 75v1152q0 40-15 75t-41 61t-61 41t-75 15H192q-40 0-75-15t-61-41t-41-61t-15-75V576q0-40 15-75t41-61t61-41t75-15h320q0-37-1-82t9-83t37-65t83-26h768q37 0 61 12t38 32t20 46t9 55t1 57t-1 54zm-1216 0h768V256H640zm1280 192q0-26-19-45t-45-19H192q-26 0-45 19t-19 45v1152q0 26 19 45t45 19h1664q26 0 45-19t19-45z" />
                </svg>

                <h5 class=" mb-2 text-2xl font-bold tracking-tight text-gray-200 dark:text-white">
                  Aura Hospital Management System</h5>
              </div>
              <p class="font-normal  text-gray-300 dark:text-gray-400">Aura HMS is a web software for an hospital that
                manages the day to day activities of the hospital. It was build with Vue.Js, NodeJs and Express server.
              </p>
              <a href="#" class="inline-flex pt-4 font-medium items-center text-gray-400 hover:underline">
                visit project
                <svg class="w-3 h-3 ms-2.5 rtl:rotate-[270deg]" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                  fill="none" viewBox="0 0 18 18">
                  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M15 11v4.833A1.166 1.166 0 0 1 13.833 17H2.167A1.167 1.167 0 0 1 1 15.833V4.167A1.166 1.166 0 0 1 2.167 3h4.618m4.447-2H17v5.768M9.111 8.889l7.778-7.778" />
                </svg>
              </a>
            </div>

          </div>
        </div>

        <div data-aos="fade-up" class="col-span-6 px-4 mt-10 md:mt-0 overflow-hidden">
          <div class="content">

            <div
              class="block max-w-full p-6 bg-gradient-to-r from-purple-700 to-pink-800 rounded shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">

              <svg class="text-gray-200" xmlns="http://www.w3.org/2000/svg" width="3em" height="3em"
                viewBox="0 0 24 24">
                <g fill="none">
                  <path
                    d="M24 0v24H0V0zM12.593 23.258l-.011.002l-.071.035l-.02.004l-.014-.004l-.071-.035q-.016-.005-.024.005l-.004.01l-.017.428l.005.02l.01.013l.104.074l.015.004l.012-.004l.104-.074l.012-.016l.004-.017l-.017-.427q-.004-.016-.017-.018m.265-.113l-.013.002l-.185.093l-.01.01l-.003.011l.018.43l.005.012l.008.007l.201.093q.019.005.029-.008l.004-.014l-.034-.614q-.005-.019-.02-.022m-.715.002a.02.02 0 0 0-.027.006l-.006.014l-.034.614q.001.018.017.024l.015-.002l.201-.093l.01-.008l.004-.011l.017-.43l-.003-.012l-.01-.01z" />
                  <path fill="currentColor"
                    d="M12 2c5.523 0 10 4.477 10 10a9.98 9.98 0 0 1-3.76 7.814l-.239.186H20a1 1 0 0 1 .117 1.993L20 22h-8C6.477 22 2 17.523 2 12S6.477 2 12 2m0 2a8 8 0 1 0 0 16a8 8 0 0 0 0-16m0 10a2 2 0 1 1 0 4a2 2 0 0 1 0-4m-4-4a2 2 0 1 1 0 4a2 2 0 0 1 0-4m8 0a2 2 0 1 1 0 4a2 2 0 0 1 0-4m-4-4a2 2 0 1 1 0 4a2 2 0 0 1 0-4" />
                </g>
              </svg>

              <h5 class="mb-2 text-2xl font-bold tracking-tight text-white dark:text-white">The MovieFusion Movie App
              </h5>
              <p class="font-normal text-gray-300 dark:text-gray-400">Moviefusion is a movie web application built with
                Vue.js and Firebase technologies. It has features like collections, movie cast, watch providers and
                youtube trailers.</p>

              <a href="#" class="inline-flex pt-4 font-medium items-center text-gray-400 hover:underline">
                visit project
                <svg class="w-3 h-3 ms-2.5 rtl:rotate-[270deg]" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                  fill="none" viewBox="0 0 18 18">
                  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M15 11v4.833A1.166 1.166 0 0 1 13.833 17H2.167A1.167 1.167 0 0 1 1 15.833V4.167A1.166 1.166 0 0 1 2.167 3h4.618m4.447-2H17v5.768M9.111 8.889l7.778-7.778" />
                </svg>
              </a>
            </div>

          </div>
        </div>

        <div data-aos="fade-down" class="col-span-6 px-4 mt-10 overflow-hidden">
          <div class="content">
            <div
              class="block max-w-full p-6 bg-gradient-to-r from-purple-700 to-pink-800 rounded shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700">
              <svg class="text-gray-200" xmlns="http://www.w3.org/2000/svg" width="3em" height="3em"
                viewBox="0 0 32 32">
                <path fill="currentColor"
                  d="M29.02 11.754L8.416 9.474L7.16 4.715a.758.758 0 0 0-.727-.558H3.34a1.214 1.214 0 0 0-.963-.49a1.24 1.24 0 1 0 0 2.483c.4 0 .738-.2.965-.492h2.512l5.23 19.8a3.282 3.282 0 0 0-.89 2.242a3.29 3.29 0 0 0 3.292 3.293a3.296 3.296 0 0 0 3.297-3.293a3.19 3.19 0 0 0-.093-.743h5.533a3.25 3.25 0 0 0-.092.743c0 1.82 1.476 3.293 3.296 3.293S28.72 29.52 28.72 27.7a3.296 3.296 0 0 0-3.294-3.297c-.95 0-1.8.41-2.402 1.053h-7.136a3.276 3.276 0 0 0-2.402-1.053c-.38 0-.738.078-1.077.196l-.182-.686H26.81a2.5 2.5 0 0 0 2.39-1.96l1.575-7.798a2.17 2.17 0 0 0 .04-.414a1.995 1.995 0 0 0-1.795-1.988zm-3.592 16.24a.298.298 0 0 1-.297-.295c.003-.166.135-.298.298-.298s.295.132.297.297a.298.298 0 0 1-.297.294zm1.78-7.495l.948-.95l-.318 1.58zm-14.453-9.037L13.79 12.5l-1.29 1.29l-1.293-1.29l1.087-1.088zm4.498.498l.538.54l-1.29 1.29l-1.293-1.29l.688-.69l1.358.15zM9.63 14.076l.87-.868l1.29 1.292l-1.29 1.29l-.565-.563l-.304-1.152zm-.295-1.12l-.328-1.24l.785.785zM21.79 16.5l-1.29 1.29l-1.293-1.29l1.292-1.293zm-.583-2l1.292-1.292l1.29 1.292l-1.29 1.292zM18.5 15.79l-1.293-1.29l1.292-1.293l1.29 1.292zm-.71.71l-1.29 1.29l-1.292-1.29l1.292-1.293zm-3.29-.71l-1.293-1.29l1.292-1.293l1.29 1.292zm-.71.71l-1.29 1.29l-1.293-1.29l1.292-1.293zm-3.29.707l1.29 1.292l-.784.783l-.54-2.044l.033-.033zm.802 3.197l1.197-1.197l1.29 1.292l-1.29 1.29l-1.13-1.13zm1.906-1.905l1.29-1.293l1.293 1.292l-1.29 1.29l-1.292-1.29zm3.292.707l1.292 1.292l-1.292 1.29l-1.292-1.29zm.708-.708l1.292-1.293l1.29 1.292l-1.29 1.29zm3.29.707l1.293 1.292l-1.29 1.29l-1.292-1.292zm.71-.708l1.29-1.293l1.293 1.292l-1.29 1.29zm2-2l1.29-1.293l1.293 1.292l-1.29 1.29zm2-2l1.29-1.293L27.79 14.5l-1.29 1.292l-1.293-1.293zm-.71-.708l-1.155-1.156l2.082.23zM21.792 12.5l-1.29 1.292l-1.293-1.292l.29-.29l2.253.25zm-7.29-.71l-.152-.15l.273.03l-.12.12zm-4 .002l-.65-.65l1.17.13zm4 9.415l1.205 1.205h-2.41zm4 0l1.205 1.206h-2.412zm4 0l1.207 1.207h-2.414zm.707-.708l1.292-1.293l1.29 1.292l-1.29 1.29zm2-2l1.292-1.292l1.29 1.29l-1.29 1.293l-1.293-1.29zm3.292-.71l-1.292-1.29l1.29-1.292l.445.444l-.43 2.124l-.014.015zm.5-4.5l-.5.5l-.66-.657l1.017.112c.054.008.1.026.144.044zM13.488 27.993a.297.297 0 0 1 0-.593a.296.296 0 0 1 0 .591zm13.323-5.58h-1.517l1.207-1.207l.93.93c-.187.17-.423.29-.62.277" />
              </svg>

              <h5 class="mb-2 text-2xl font-bold tracking-tight text-white dark:text-white">ShoppersNg Ecommerce App
              </h5>
              <p class="font-normal text-gray-300 dark:text-gray-400">ShopppersNg is an Ecommerce web application built
                with VueJs and fakestore api. It has store and add to cart feature.</p>

              <a href="#" class="inline-flex pt-4 font-medium items-center text-gray-400 hover:underline">
                visit project
                <svg class="w-3 h-3 ms-2.5 rtl:rotate-[270deg]" aria-hidden="true" xmlns="http://www.w3.org/2000/svg"
                  fill="none" viewBox="0 0 18 18">
                  <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M15 11v4.833A1.166 1.166 0 0 1 13.833 17H2.167A1.167 1.167 0 0 1 1 15.833V4.167A1.166 1.166 0 0 1 2.167 3h4.618m4.447-2H17v5.768M9.111 8.889l7.778-7.778" />
                </svg>
              </a>
            </div>


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
