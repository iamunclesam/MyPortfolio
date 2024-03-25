<template>
  <section class=" dark:bg-gray-900">
    <div
      class="grid order-1 md:order-1 max-w-screen-xl md:px-28 px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12">
      <div class="md:hidden md:order-2 lg:mt-0 lg:col-span-5 md:flex">
        <img src="@/assets/img/sam.png"
          class="w-64 mx-auto my-6 mb-10 rounded-full border glow-neon-button border-green-600" alt="mockup">
      </div>
      <div class="mr-auto place-self-center lg:col-span-7">
        <span
          class="bg-green-300 text-green-800 text-xs font-medium me-2 px-2.5 py-0.5 mb-8 rounded dark:bg-green-900 dark:text-green-300">Web
          App Developer</span>
        <h1
          class="max-w-2xl my-4 text-4xl font-medium tracking-tight text-white leading-none md:text-5xl xl:text-6xl dark:text-white">
          { Hello World! }</h1>
        <h1
          class="max-w-2xl mb-4 text-4xl font-medium tracking-tight text-white leading-none md:text-5xl xl:text-6xl dark:text-white">
          I'm Samuel Adeyemi</h1>
        <p class="max-w-2xl mb-6 font-light text-gray-500 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400">I'm a
          creative web app developer with rock-solid experience to build simple and complex web applications with recent
          technologies.</p>
        <a href="#"
          class="inline-flex items-center justify-center px-3 border border-gray-300 py-3 mr-3 text-base font-medium text-center text-green-500 rounded-lg bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 dark:focus:ring-primary-900">
          Download My CV
          <svg class="w-5 h-5 ml-2 -mr-1" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg">
            <path fill-rule="evenodd"
              d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
              clip-rule="evenodd"></path>
          </svg>
        </a>

      
        <!-- <a href="#" class="inline-flex items-center justify-center px-5 py-3 text-base font-medium text-center text-gray-900 border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:ring-gray-100 dark:text-white dark:border-gray-700 dark:hover:bg-gray-700 dark:focus:ring-gray-800">
                Speak to Sales
            </a>  -->
      </div>
      <div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
        <img src="@/assets/img/sam.png" class="w-full rounded-full border glow-neon-button border-green-600"
          alt="mockup">
      </div>
    </div>
  </section>
</template>

<script>
</script>

<style>
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
