<script>
import Hero from '@/components/Layout/hero.vue'
import Navbar from '@/components/Layout/navbar.vue'
export default {

  components: {
    Navbar, Hero
  }
}

</script>

<template>

  <main>
    <Navbar />
    <Hero />

    <div class="about px-4 md:px-28 my-10">
      <div class="grid md:grid-cols-12">
        <div class="col-span-6 order-2 md:order-1 px-auto md:p-8">
          <div class="content">
            <div class="box mb-2 p-6 w-74 shadow-lg">
             <div class="flex justify-between h-auto items-center">
              <h1 class="text-green-600 font-bold">Design</h1>
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24" class="text-green-600" ><path fill="currentColor" d="M3 17.25V21h3.75L17.81 9.93l-3.75-3.75zm19.61 1.11l-4.25 4.25l-5.2-5.2l1.77-1.77l1 1l2.47-2.48l1.42 1.42L18.36 17l1.06 1l1.42-1.4zm-16-7.53L1.39 5.64l4.25-4.25L7.4 3.16L4.93 5.64L6 6.7l2.46-2.48l1.42 1.42l-1.42 1.41l1 1zM20.71 7c.39-.39.39-1 0-1.41l-2.34-2.3c-.37-.39-1.02-.39-1.41 0l-1.84 1.83l3.75 3.75z"/></svg>
             </div>
              <p class="text-gray-700 text-sm font-medium text-gray-500">Lorem ipsum, dolor sit amet consectetur
                adipisicing elit.</p>
            </div>

           

            <div class="box mb-2 p-6 w-74 shadow-lg">
              <div class="flex justify-between h-auto items-center">
              <h1 class="text-green-600 font-bold">Front-end</h1>
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" class="text-green-600" viewBox="0 0 24 24"><g fill="none"><path d="M0 0h24v24H0z"/><path fill="currentColor" d="M14.62 2.662a1.5 1.5 0 0 1 1.04 1.85l-4.431 15.787a1.5 1.5 0 0 1-2.889-.81L12.771 3.7a1.5 1.5 0 0 1 1.85-1.039ZM7.56 6.697a1.5 1.5 0 0 1 0 2.12L4.38 12l3.182 3.182a1.5 1.5 0 1 1-2.122 2.121L1.197 13.06a1.5 1.5 0 0 1 0-2.12l4.242-4.243a1.5 1.5 0 0 1 2.122 0Zm8.88 2.12a1.5 1.5 0 1 1 2.12-2.12l4.243 4.242a1.5 1.5 0 0 1 0 2.121l-4.242 4.243a1.5 1.5 0 1 1-2.122-2.121L19.621 12z"/></g></svg>
             </div>
              <p class="text-gray-700 text-sm font-medium text-gray-500">Lorem ipsum, dolor sit amet consectetur
                adipisicing elit.</p>
            </div>

           

            <div class="box p-6 w-74 shadow-lg">
              <div class="flex justify-between h-auto items-center">
              <h1 class="text-green-600 font-bold">Back-end</h1>
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" class="text-green-600" viewBox="0 0 20 20"><path id="oouiCode0" fill="currentColor" d="M1 10.08V8.92h1.15c1.15 0 1.15 0 1.15-1.15V5a7.4 7.4 0 0 1 .09-1.3a2 2 0 0 1 .3-.7a1.84 1.84 0 0 1 .93-.68A6.4 6.4 0 0 1 6.74 2h1.18v1.15h-.86A1.32 1.32 0 0 0 6 3.62a1.7 1.7 0 0 0-.36 1.23V7a3.2 3.2 0 0 1-.28 1.72a2 2 0 0 1-1.26.77a2.15 2.15 0 0 1 1.26.79A3.26 3.26 0 0 1 5.62 12v3.15A1.67 1.67 0 0 0 6 16.37a1.31 1.31 0 0 0 1.08.47h.87V18H6.74a6.3 6.3 0 0 1-2.12-.29a1.82 1.82 0 0 1-.93-.71a1.9 1.9 0 0 1-.3-.72A7.5 7.5 0 0 1 3.31 15v-3.77c0-1.15 0-1.15-1.15-1.15zm18 0V8.92h-1.15c-1.15 0-1.15 0-1.15-1.15V5a7.4 7.4 0 0 0-.08-1.32a2 2 0 0 0-.3-.73a1.84 1.84 0 0 0-.93-.68A6.4 6.4 0 0 0 13.26 2h-1.18v1.15h.87a1.32 1.32 0 0 1 1.05.47a1.7 1.7 0 0 1 .36 1.23V7a3.2 3.2 0 0 0 .28 1.72a2 2 0 0 0 1.26.77a2.15 2.15 0 0 0-1.26.79a3.26 3.26 0 0 0-.26 1.72v3.15a1.67 1.67 0 0 1-.38 1.22a1.31 1.31 0 0 1-1.08.47h-.87V18h1.19a6.3 6.3 0 0 0 2.12-.29a1.82 1.82 0 0 0 .93-.68a1.9 1.9 0 0 0 .3-.72a7.5 7.5 0 0 0 .1-1.31v-3.77c0-1.15 0-1.15 1.15-1.15z"/><use href="#oouiCode0" transform="matrix(-1 0 0 1 20 0)"/></svg>
             </div>
              <p class="text-gray-700 text-sm font-medium text-gray-500">Lorem ipsum, dolor sit amet consectetur
                adipisicing elit.</p>
            </div>
          </div>
        </div>

        <div class="col-span-6 order-1 md:order-2">
          <div class="content md:p-16 pb-8">
            <h1 class="text-green-400 text-sm ">Lorem, ipsum</h1>
            <h1 class="text-2xl font-light text-white">Lorem ipsum, dolor sit amet consectetur.</h1>
            <p class="text-gray-500 py-4 text-sm">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id dolorem
              porro quasi cupiditate. Harum cum veniam magnam necessitatibus fugiat vel.</p>

            <p class="text-gray-500 hidden md:block text-sm">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Id dolorem porro
              quasi cupiditate. Harum cum veniam magnam necessitatibus fugiat vel.</p>
          </div>
        </div>
      </div>
    </div>

    <div class="projects md:px-28 px-4 my-10">
      <div class="grid md:grid-cols-12">
        <div class="col-span-6 px-4">
          <div class="content">
            <h1 class="text-right text-3xl font-light text-green-600">Latest Work</h1>
            <div class="grid md:grid-cols-2 my-10">
              <div class="col">
                <img src="@/assets/img/p1.png" class="w-96" alt="mockup">
              </div>

              <div class="col">
                <div class="content">
                  <div class="h1 text-green-500 text-3xl font-light">MovieFusion Movie App</div>
                  <p class="text-gray-500 font-medium py-4 text-sm">Lorem, ipsum dolor sit amet consectetur adipisicing
                    elit. Dolorem soluta assumenda optio voluptates dolor. Eligendi odio saepe modi necessitatibus
                    blanditiis.</p>
                  <button
                    class="glow-neon-button bg-green-700 text-white font-light py-1.5 text-sm px-4 rounded-md shadow-md hover:shadow-lg">Visit
                    site</button>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-span-6">
          <div class="content md:mt-64">

            <div class="grid md:grid-cols-2 my-10">
              <div class="col">
                <img src="@/assets/img/p2.png" class="w-96" alt="mockup">
              </div>

              <div class="col">
                <div class="content">
                  <div class="h1 text-green-500 text-3xl font-light">Shoppers E-commerce App</div>
                  <p class="text-gray-500 font-medium py-4 text-sm">Lorem, ipsum dolor sit amet consectetur adipisicing
                    elit. Dolorem soluta assumenda optio voluptates dolor. Eligendi odio saepe modi necessitatibus
                    blanditiis.</p>
                  <button
                    class="glow-neon-button bg-green-700 text-white font-light py-1.5 text-sm px-4 rounded-md shadow-md hover:shadow-lg">Visit
                    site</button>

                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-span-6 px-4">
          <div class="content">
            <div class="grid md:grid-cols-2 my-10">
              <div class="col">
                <img src="@/assets/img/p3.png" class="w-96" alt="mockup">
              </div>

              <div class="col">
                <div class="content">
                  <div class="h1 text-green-500 text-3xl font-light">College Department App</div>
                  <p class="text-gray-500 font-medium py-4 text-sm">Lorem, ipsum dolor sit amet consectetur adipisicing
                    elit. Dolorem soluta assumenda optio voluptates dolor. Eligendi odio saepe modi necessitatibus
                    blanditiis.</p>
                  <button
                    class="glow-neon-button bg-green-700 text-white font-light py-1.5 text-sm px-4 rounded-md shadow-md hover:shadow-lg">Visit
                    site</button>

                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-span-6 px-4 md:relative">
          <div class="content md:absolute bottom-20 right-20">
            <div class="text-green-500 text-md font-light underline">VIEW ALL PROJECTS</div>
            <p class="text-gray-500 w-32 pt-8 text-sm font-light">Lorem ipsum dolor sit amet consectetur.</p>
          </div>
        </div>


      </div>
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
  box-shadow: 0 0 20px #147650, 0 0 40px #147650, 0 0 60px #147650, 0 0 80px #147650;
  animation: glow-neon-animation 1s ease-in-out infinite alternate;
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
