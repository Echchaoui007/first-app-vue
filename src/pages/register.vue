
<template>
    <div class="flex flex-col items-center">
      <form class="bg-white p-6 rounded-lg shadow-md" @submit.prevent="submitForm">
        <h2 class="text-lg font-medium mb-4">
          Register
        </h2>
        <div class="mb-4">
          <label class="block text-gray-700 font-medium mb-2" for="email">
            UserName:
          </label>
          <input
            v-model="formData.email"
            class="bg-gray-200 appearance-none border-2 border-gray-200 rounded w-full py-2 px-4 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
            id="email"
            type="email"
          />
        </div>
        <div class="mb-4">
          <label class="block text-gray-700 font-medium mb-2" for="password">
            Email:
          </label>
          <input
            v-model="formData.password"
            class="bg-gray-200 appearance-none border-2 border-gray-200 rounded w-full py-2 px-4 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
            id="password"
            type="password"
          />
        </div>
        <div class="mb-4" hidden>
          <label class="block text-gray-700 font-medium mb-2" for="password_confirmation">
            Your pass_key
          </label>
          <input
            v-model="formData.pass_key"
            class="bg-gray-200 appearance-none border-2 border-gray-200 rounded w-full py-2 px-4 text-gray-700 leading-tight focus:outline-none focus:bg-white focus:border-purple-500"
            id="password_confirmation"
            type="password"
          />
        </div>
        <div class="flex items-center justify-between">
          <button
            class="bg-purple-500 hover:bg-purple-700 text-white font-medium py-2 px-4 rounded focus:outline-none focus:shadow-outline"
            type="submit"
          >
            Register
          </button>
        </div>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        formData: {
            username: '',
            email: '',
        }
      }
    },
    methods: {
      submitForm() {
        // handle form submission, for example using axios
      }
    }
  }
  </script>
  