<template>
  <nav class="bg-white">
    <div class="container mx-auto px-4">
      <div class="flex items-center justify-between h-20">
        <img
          class=""
          src="@/assets/images/logo.svg"
          alt="Workflow logo"
          style="width: 100%; max-width: 180px"
        />

        <div class="hidden md:block">
          <div class="mx-4 flex items-baseline">
            <a
              href="#"
              class="px-3 py-2 rounded text-md font-medium text-primary focus:outline-none focus:text-primary whitespace-no-wrap"
              >Página inicial</a
            >
            <a
              href="#"
              class="ml-4 px-3 py-2 rounded text-md font-medium text-gray-800 hover:text-primary-400 focus:outline-none focus:text-white whitespace-no-wrap"
              >Sobre nós</a
            >
            <a
              href="#"
              class="ml-4 px-3 py-2 rounded text-md font-medium text-gray-800 hover:text-primary-400 focus:outline-none focus:text-white whitespace-no-wrap"
              >PetCode</a
            >
            <a
              href="#"
              class="ml-4 px-3 py-2 rounded text-md font-medium text-gray-800 hover:text-primary-400 focus:outline-none focus:text-white whitespace-no-wrap"
              >Contato</a
            >
          </div>
        </div>

        <div class="hidden md:block">
          <div class="ml-4 flex items-center">
            <button
              class="bg-white border border-primary text-primary hover:text-white hover:bg-primary-500 hover:border-primary-500 px-6 py-2 rounded text-md font-medium whitespace-no-wrap mr-2"
            >
              Entrar
            </button>
            <button
              class="bg-primary border border-primary text-white px-6 py-2 rounded text-md font-medium whitespace-no-wrap hover:bg-primary-500"
            >
              Criar conta
            </button>
          </div>
        </div>
        <div class="-mr-2 flex md:hidden">
          <!-- Mobile menu button -->
          <button
            @click="toggle"
            class="inline-flex items-center justify-center p-2 rounded text-primary hover:text-white hover:bg-primary focus:outline-none focus:bg-primary focus:text-white"
          >
            <svg
              :class="[isOpen ? 'hidden' : 'block', 'h-4 w-4']"
              stroke="currentColor"
              fill="none"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M4 6h16M4 12h16M4 18h16"
              ></path>
            </svg>
            <svg
              :class="[isOpen ? 'block' : 'hidden', 'h-4 w-4']"
              stroke="currentColor"
              fill="none"
              viewBox="0 0 24 24"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M6 18L18 6M6 6l12 12"
              ></path>
            </svg>
          </button>
        </div>
      </div>
    </div>
    <div :class="[isOpen ? '' : 'hidden', 'md:hidden']">
      <div class="px-2 pt-2 pb-3 sm:px-3">
        <a
          href="#"
          class="block px-3 py-2 rounded text-base font-medium text-white bg-gray-900 focus:outline-none focus:text-white focus:bg-gray-700"
          >Dashboard</a
        >
        <a
          href="#"
          class="mt-1 block px-3 py-2 rounded text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
          >Team</a
        >
        <a
          href="#"
          class="mt-1 block px-3 py-2 rounded text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
          >Projects</a
        >
        <a
          href="#"
          class="mt-1 block px-3 py-2 rounded text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
          >Calendar</a
        >
        <a
          href="#"
          class="mt-1 block px-3 py-2 rounded text-base font-medium text-gray-300 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
          >Reports</a
        >
      </div>
      <div class="pt-4 pb-3 border-t border-gray-700">
        <div class="flex items-center px-5">
          <div class="flex-shrink-0">
            <img
              class="h-10 w-10 rounded-full"
              src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80"
              alt
            />
          </div>
          <div class="ml-3">
            <div class="text-base font-medium leading-none text-white">
              Tom Cook
            </div>
            <div class="mt-1 text-sm font-medium leading-none text-gray-400">
              tom@example.com
            </div>
          </div>
        </div>
        <div class="mt-3 px-2">
          <a
            href="#"
            class="block px-3 py-2 rounded text-base font-medium text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
            >Your Profile</a
          >
          <a
            href="#"
            class="mt-1 block px-3 py-2 rounded text-base font-medium text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
            >Settings</a
          >
          <a
            href="#"
            class="mt-1 block px-3 py-2 rounded text-base font-medium text-gray-400 hover:text-white hover:bg-gray-700 focus:outline-none focus:text-white focus:bg-gray-700"
            >Sign out</a
          >
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
    },
  },
};
</script>
