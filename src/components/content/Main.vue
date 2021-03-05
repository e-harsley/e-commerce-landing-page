<template>
  <div class="mt-16">
    <h3 class="text-gray-600 text-2xl font-medium">Merchants</h3>
    <div id="myBtnContainer" class="my-6">
      <button
        :class="{ active: active_tab === 'all' }"
        class="btn px-5 py-3 mr-2 rounded bg-gray-200 hover:bg-gray-900 hover:text-white my-1 text-gray-600"
        @click="filterSelection('all')"
      >
        All Merchants
      </button>
      <button
        :class="{ active: active_tab === 'service' }"
        class="btn px-5 py-3 mr-2 rounded bg-gray-200 hover:bg-gray-900 hover:text-white my-1 text-gray-600"
        @click="filterSelection('service')"
      >
        Service Merchants
      </button>
      <button
        :class="{ active: active_tab === 'product' }"
        class="btn px-5 py-3 mr-2 rounded bg-gray-200 hover:bg-gray-900 hover:text-white my-1 text-gray-600"
        @click="filterSelection('product')"
      >
        Product Merchants
      </button>
    </div>
    <div
      class="grid gap-6 grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 mt-6 containers"
    >
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1563170351-be82bc888aa4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=376&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Chanel</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden service column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1544441893-675973e31985?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Man Mix</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden service column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1590664863685-a99ef05e9f61?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=345&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">woman mix</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1563170351-be82bc888aa4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=376&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Chanel</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden service column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1544441893-675973e31985?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Man Mix</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden service column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden service column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden service column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden service column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1532667449560-72a95c8d381b?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">Classic watch</h3>
        </div>
      </div>
      <div
        class="w-full max-w-sm mx-auto rounded-md shadow-md overflow-hidden product column"
      >
        <div
          class="flex items-end justify-end h-56 w-full bg-cover"
          style="background-image: url('https://images.unsplash.com/photo-1590664863685-a99ef05e9f61?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=345&q=80')"
        >
          <button
            class="p-2 rounded-full bg-blue-600 text-white mx-5 -mb-4 hover:bg-blue-500 focus:outline-none focus:bg-blue-500"
          >
            <svg
              class="h-5 w-5"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                d="M3 3h2l.4 2M7 13h10l4-8H5.4M7 13L5.4 5M7 13l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17m0 0a2 2 0 100 4 2 2 0 000-4zm-8 2a2 2 0 11-4 0 2 2 0 014 0z"
              ></path>
            </svg>
          </button>
        </div>
        <div class="px-5 py-3">
          <h3 class="text-gray-700 uppercase">woman mix</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      active_tab: "all",
    };
  },
  methods: {
    filterSelection(data) {
      const x = document.getElementsByClassName("column");

      for (let i = 0; i < x.length; i++) {
        x[i].style.display = "";
        if (data == "all") {
          x[i].style.display = "";
          this.active_tab = data;
        } else {
          if (x[i].classList.contains(data) == false) {
            x[i].style.display = "none";
            this.active_tab = data;
          }
        }
      }
    },
  },
};
</script>

<style></style>
