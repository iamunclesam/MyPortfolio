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




    <div class="about px-4 md:px-28 my-10">
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
              <p class="text-gray-700 text-sm font-medium text-gray-500">Proeficient in responsive applications for better user experience.</p>
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
              <p class="text-gray-700 text-sm font-medium text-gray-500">Proeficient in backend technologies around NodeJs.</p>
            </div>
          </div>
        </div>

        <div data-aos="fade-left" class="col-span-6 order-1 md:order-2">
          <div class="content md:p-16 pb-8">
            <code class="text-purple-500 text-sm "> About Unclesam </code>
            <h1 class="text-2xl font-light text-white">Get a peek into my career journey</h1>
            <p class="text-gray-500 py-4 text-sm">I'm Samuel Adeyemi a.k.a <span class="text-purple-600">Unclesam</span>, a web app developer with 3 years of experience. Specializing in Vue.js for frontend and Node.js with Firebase for backend, I've collaborated with startups, crafting intuitive solutions that resonate with users.</p>

            <p class="text-gray-500 hidden md:block text-sm">Innovation drives me. Let's connect to create impactful web experiences that shape the future.</p>

            <a href="#"
          class="inline-flex items-center justify-center py-3 mr-3 text-base font-medium text-center text-purple-500 rounded-lg bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900">
          let's connect
          <svg class="w-5 h-5 ml-2 -mr-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
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
      <h1 class="text-right md:text-center md:text-white text-3xl font-light text-white">Latest Work</h1>
      <div class="grid md:grid-cols-12">
        <div data-aos="fade-right" class="col-span-6 px-4">
          <div class="content">

            <div class="grid md:grid-cols-2 my-10">
              <div class="col">
                <img src="@/assets/img/p1.png" class="w-96" alt="mockup">
              </div>

              <div class="col">
                <div class="content">
                  <div class="h1 text-purple-600 text-3xl font-light">MovieFusion Movie App</div>
                  <p class="text-gray-500 font-medium py-4 text-sm">Moviefuison is demo movie app built with VueJs with features like movie collections and favourites. Your contribution is appreciated!</p>
                  <div class="github mb-6">
                    <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em" viewBox="0 0 256 256">
                      <g fill="none">
                        <rect width="256" height="256" fill="#242938" rx="60" />
                        <path fill="#fff"
                          d="M128.001 30C72.779 30 28 74.77 28 130.001c0 44.183 28.653 81.667 68.387 94.89c4.997.926 6.832-2.169 6.832-4.81c0-2.385-.093-10.262-.136-18.618c-27.82 6.049-33.69-11.799-33.69-11.799c-4.55-11.559-11.104-14.632-11.104-14.632c-9.073-6.207.684-6.079.684-6.079c10.042.705 15.33 10.305 15.33 10.305c8.919 15.288 23.394 10.868 29.1 8.313c.898-6.464 3.489-10.875 6.349-13.372c-22.211-2.529-45.56-11.104-45.56-49.421c0-10.918 3.906-19.839 10.303-26.842c-1.039-2.519-4.462-12.69.968-26.464c0 0 8.398-2.687 27.508 10.25c7.977-2.215 16.531-3.326 25.03-3.364c8.498.038 17.06 1.149 25.051 3.365c19.087-12.939 27.473-10.25 27.473-10.25c5.443 13.773 2.019 23.945.98 26.463c6.412 7.003 10.292 15.924 10.292 26.842c0 38.409-23.394 46.866-45.662 49.341c3.587 3.104 6.783 9.189 6.783 18.519c0 13.38-.116 24.149-.116 27.443c0 2.661 1.8 5.779 6.869 4.797C199.383 211.64 228 174.169 228 130.001C228 74.771 183.227 30 128.001 30M65.454 172.453c-.22.497-1.002.646-1.714.305c-.726-.326-1.133-1.004-.898-1.502c.215-.512.999-.654 1.722-.311c.727.326 1.141 1.01.89 1.508m4.919 4.389c-.477.443-1.41.237-2.042-.462c-.654-.697-.777-1.629-.293-2.078c.491-.442 1.396-.235 2.051.462c.654.706.782 1.631.284 2.078m3.374 5.616c-.613.426-1.615.027-2.234-.863c-.613-.889-.613-1.955.013-2.383c.621-.427 1.608-.043 2.236.84c.611.904.611 1.971-.015 2.406m5.707 6.504c-.548.604-1.715.442-2.57-.383c-.874-.806-1.118-1.95-.568-2.555c.555-.606 1.729-.435 2.59.383c.868.804 1.133 1.957.548 2.555m7.376 2.195c-.242.784-1.366 1.14-2.499.807c-1.13-.343-1.871-1.26-1.642-2.052c.235-.788 1.364-1.159 2.505-.803c1.13.341 1.871 1.252 1.636 2.048m8.394.932c.028.824-.932 1.508-2.121 1.523c-1.196.027-2.163-.641-2.176-1.452c0-.833.939-1.51 2.134-1.53c1.19-.023 2.163.639 2.163 1.459m8.246-.316c.143.804-.683 1.631-1.864 1.851c-1.161.212-2.236-.285-2.383-1.083c-.144-.825.697-1.651 1.856-1.865c1.183-.205 2.241.279 2.391 1.097" />
                      </g>
                    </svg>
                  </div>
                  <button
                    class=" bg-purple-700 text-white font-light py-1.5 text-sm px-4 rounded-md shadow-md hover:shadow-lg">Visit
                    site</button>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div data-aos="fade-left" class="col-span-6 px-4">
          <div class="content md:mt-64">

            <div class="grid md:grid-cols-2 my-10">
              <div class="col">
                <img src="@/assets/img/p2.png" class="w-96" alt="mockup">
              </div>

              <div class="col">
                <div class="content">
                  <div class="h1 text-purple-600 text-3xl font-light">Shoppers E-commerce App</div>
                  <p class="text-gray-500 font-medium py-4 text-sm">ShoppersNg is also demo ecommerce app built with VueJs and third party Api (fakestoreapi) with add to cart feature and product details page. Your contribution is appreciated</p>
                  <div class="github mb-6">
                    <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em" viewBox="0 0 256 256">
                      <g fill="none">
                        <rect width="256" height="256" fill="#242938" rx="60" />
                        <path fill="#fff"
                          d="M128.001 30C72.779 30 28 74.77 28 130.001c0 44.183 28.653 81.667 68.387 94.89c4.997.926 6.832-2.169 6.832-4.81c0-2.385-.093-10.262-.136-18.618c-27.82 6.049-33.69-11.799-33.69-11.799c-4.55-11.559-11.104-14.632-11.104-14.632c-9.073-6.207.684-6.079.684-6.079c10.042.705 15.33 10.305 15.33 10.305c8.919 15.288 23.394 10.868 29.1 8.313c.898-6.464 3.489-10.875 6.349-13.372c-22.211-2.529-45.56-11.104-45.56-49.421c0-10.918 3.906-19.839 10.303-26.842c-1.039-2.519-4.462-12.69.968-26.464c0 0 8.398-2.687 27.508 10.25c7.977-2.215 16.531-3.326 25.03-3.364c8.498.038 17.06 1.149 25.051 3.365c19.087-12.939 27.473-10.25 27.473-10.25c5.443 13.773 2.019 23.945.98 26.463c6.412 7.003 10.292 15.924 10.292 26.842c0 38.409-23.394 46.866-45.662 49.341c3.587 3.104 6.783 9.189 6.783 18.519c0 13.38-.116 24.149-.116 27.443c0 2.661 1.8 5.779 6.869 4.797C199.383 211.64 228 174.169 228 130.001C228 74.771 183.227 30 128.001 30M65.454 172.453c-.22.497-1.002.646-1.714.305c-.726-.326-1.133-1.004-.898-1.502c.215-.512.999-.654 1.722-.311c.727.326 1.141 1.01.89 1.508m4.919 4.389c-.477.443-1.41.237-2.042-.462c-.654-.697-.777-1.629-.293-2.078c.491-.442 1.396-.235 2.051.462c.654.706.782 1.631.284 2.078m3.374 5.616c-.613.426-1.615.027-2.234-.863c-.613-.889-.613-1.955.013-2.383c.621-.427 1.608-.043 2.236.84c.611.904.611 1.971-.015 2.406m5.707 6.504c-.548.604-1.715.442-2.57-.383c-.874-.806-1.118-1.95-.568-2.555c.555-.606 1.729-.435 2.59.383c.868.804 1.133 1.957.548 2.555m7.376 2.195c-.242.784-1.366 1.14-2.499.807c-1.13-.343-1.871-1.26-1.642-2.052c.235-.788 1.364-1.159 2.505-.803c1.13.341 1.871 1.252 1.636 2.048m8.394.932c.028.824-.932 1.508-2.121 1.523c-1.196.027-2.163-.641-2.176-1.452c0-.833.939-1.51 2.134-1.53c1.19-.023 2.163.639 2.163 1.459m8.246-.316c.143.804-.683 1.631-1.864 1.851c-1.161.212-2.236-.285-2.383-1.083c-.144-.825.697-1.651 1.856-1.865c1.183-.205 2.241.279 2.391 1.097" />
                      </g>
                    </svg>
                  </div>
                  <button
                    class="bg-purple-700 text-white font-light py-1.5 text-sm px-4 rounded-md shadow-md hover:shadow-lg">Visit
                    site</button>

                </div>
              </div>
            </div>
          </div>
        </div>

        <div data-aos="fade-right" class="col-span-6 px-4">
          <div class="content">
            <div class="grid md:grid-cols-2 my-10">
              <div class="col">
                <img src="@/assets/img/p3.png" class="w-96" alt="mockup">
              </div>

              <div class="col">
                <div class="content">
                  <div class="h1 text-purple-600 text-3xl font-light">College Department App</div>
                  <p class="text-gray-500 font-medium py-4 text-sm">Lorem, ipsum dolor sit amet consectetur adipisicing
                    elit. Dolorem soluta assumenda optio voluptates dolor. Eligendi odio saepe modi necessitatibus
                    blanditiis.</p>
                  <div class="github mb-6">
                    <svg xmlns="http://www.w3.org/2000/svg" width="2em" height="2em" viewBox="0 0 256 256">
                      <g fill="none">
                        <rect width="256" height="256" fill="#242938" rx="60" />
                        <path fill="#fff"
                          d="M128.001 30C72.779 30 28 74.77 28 130.001c0 44.183 28.653 81.667 68.387 94.89c4.997.926 6.832-2.169 6.832-4.81c0-2.385-.093-10.262-.136-18.618c-27.82 6.049-33.69-11.799-33.69-11.799c-4.55-11.559-11.104-14.632-11.104-14.632c-9.073-6.207.684-6.079.684-6.079c10.042.705 15.33 10.305 15.33 10.305c8.919 15.288 23.394 10.868 29.1 8.313c.898-6.464 3.489-10.875 6.349-13.372c-22.211-2.529-45.56-11.104-45.56-49.421c0-10.918 3.906-19.839 10.303-26.842c-1.039-2.519-4.462-12.69.968-26.464c0 0 8.398-2.687 27.508 10.25c7.977-2.215 16.531-3.326 25.03-3.364c8.498.038 17.06 1.149 25.051 3.365c19.087-12.939 27.473-10.25 27.473-10.25c5.443 13.773 2.019 23.945.98 26.463c6.412 7.003 10.292 15.924 10.292 26.842c0 38.409-23.394 46.866-45.662 49.341c3.587 3.104 6.783 9.189 6.783 18.519c0 13.38-.116 24.149-.116 27.443c0 2.661 1.8 5.779 6.869 4.797C199.383 211.64 228 174.169 228 130.001C228 74.771 183.227 30 128.001 30M65.454 172.453c-.22.497-1.002.646-1.714.305c-.726-.326-1.133-1.004-.898-1.502c.215-.512.999-.654 1.722-.311c.727.326 1.141 1.01.89 1.508m4.919 4.389c-.477.443-1.41.237-2.042-.462c-.654-.697-.777-1.629-.293-2.078c.491-.442 1.396-.235 2.051.462c.654.706.782 1.631.284 2.078m3.374 5.616c-.613.426-1.615.027-2.234-.863c-.613-.889-.613-1.955.013-2.383c.621-.427 1.608-.043 2.236.84c.611.904.611 1.971-.015 2.406m5.707 6.504c-.548.604-1.715.442-2.57-.383c-.874-.806-1.118-1.95-.568-2.555c.555-.606 1.729-.435 2.59.383c.868.804 1.133 1.957.548 2.555m7.376 2.195c-.242.784-1.366 1.14-2.499.807c-1.13-.343-1.871-1.26-1.642-2.052c.235-.788 1.364-1.159 2.505-.803c1.13.341 1.871 1.252 1.636 2.048m8.394.932c.028.824-.932 1.508-2.121 1.523c-1.196.027-2.163-.641-2.176-1.452c0-.833.939-1.51 2.134-1.53c1.19-.023 2.163.639 2.163 1.459m8.246-.316c.143.804-.683 1.631-1.864 1.851c-1.161.212-2.236-.285-2.383-1.083c-.144-.825.697-1.651 1.856-1.865c1.183-.205 2.241.279 2.391 1.097" />
                      </g>
                    </svg>
                  </div>
                  <button
                    class="bg-purple-700 text-white font-light py-1.5 text-sm px-4 rounded-md shadow-md hover:shadow-lg">Visit
                    site</button>

                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-span-6 px-4 md:relative">
          <div class="content md:absolute bottom-20 right-20">
            <div class="text-purple-600 text-md font-light underline">VIEW ALL PROJECTS</div>
            <p class="text-gray-500 pt-8 text-sm font-medium">Take a visit to my github repo</p>
          </div>
        </div>


      </div>
    </div>

    <div class="my-skills py-20">
      <Skills />
    </div>


    <div class="socials my-20">
      <SocialLife />
    </div>


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
