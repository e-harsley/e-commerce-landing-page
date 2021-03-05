<template>
  <main class="my-8">
    <div class="container mx-auto px-6">
      <div
        class="h-96 bg-cover bg-center rounded-md overflow-hidden bg-cover bg-center"
        style="background-image: url('https://images.unsplash.com/photo-1472851294608-062f824d29cc?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1650&q=80')"
      >
        <div class="bg-gray-900 bg-opacity-50 flex items-center h-full">
          <div class="px-10 max-w-xl">
            <h2 class="text-2xl text-white font-semibold">9pay Shop</h2>
            <p class="mt-2 text-gray-400">
              Lorem ipsum dolor, sit amet consectetur adipisicing elit. Tempore
              facere provident molestias ipsam sint voluptatum pariatur.
            </p>
            <button
              class="flex items-center mt-4 px-3 py-2 bg-blue-600 text-white text-sm uppercase font-medium rounded hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
            >
              <span>Shop Now</span>
              <svg
                class="h-5 w-5 mx-2"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path d="M17 8l4 4m0 0l-4 4m4-4H3"></path>
              </svg>
            </button>
          </div>
        </div>
      </div>
      <Main />
    </div>
  </main>
</template>

<script>
import Main from "./content/Main";
export default {
  components: {
    Main,
  },
};
</script>

<style></style>
