<template>
    <nav class="flex items-center justify-between flex-wrap bg-teal-500 p-6">
      <div class="flex items-center flex-shrink-0 text-white mr-6">
        <img src="logo.png" alt="logo" class="h-8 w-8"/>
        <span class="font-semibold text-xl tracking-tight">My App</span>
      </div>
      <div class="w-full block flex-grow lg:flex lg:items-center lg:w-auto">
        <div class="text-sm lg:flex-grow">
          <a href="#" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-4">
            Home
          </a>
          <a href="#" class="block mt-4 lg:inline-block lg:mt-0 text-teal-200 hover:text-white mr-4">
            Reservation
          </a>
        </div>
        <div>
          <div class="relative">
            <button @click="isOpen = !isOpen" class="text-teal-200 hover:text-white">
              Login/Register <i class="fas fa-caret-down ml-1"></i>
            </button>
            <div v-if="isOpen" class="absolute right-0 mt-2 py-2 bg-white rounded shadow">
              <a href="#" class="block px-4 py-2 text-gray-800 hover:bg-teal-500 hover:text-white">Login</a>
              <a href="#" class="block px-4 py-2 text-gray-800 hover:bg-teal-500 hover:text-white">Register</a>
            </div>
          </div>
        </div>
      </div>
    </nav>
  </template>
  
  <script>
  export default {
    data() {
      return {
        isOpen: false
      }
    }
  }
  </script>
  