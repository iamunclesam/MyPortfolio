<template>
    <div v-if="isLoading" class="fixed top-0 left-0 w-full h-full flex items-center justify-center bg-gray-900 bg-opacity-50 z-50">
      <div class="loader ease-linear rounded-full border-8" :style="{ 'border-top-color': color, 'border-left-color': color }"></div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      isLoading: {
        type: Boolean,
        required: true
      },
      color: {
        type: String,
        default: '#38a169' // Default color (green-600)
      }
    },
    data() {
      return {
        internalLoading: false
      };
    },
    watch: {
      isLoading(newValue) {
        if (newValue) {
          // Start timer to turn off loading after 3 seconds
          this.internalLoading = true;
          setTimeout(() => {
            this.internalLoading = false;
          }, 3000); // 3 seconds
        }
      }
    }
  };
  </script>
  
  <style>
  @keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }
  
  .loader {
    border-top-color: #38a169; /* Default color */
    border-left-color: #38a169; /* Default color */
    animation: spin 1.5s linear infinite;
  }
  </style>
  