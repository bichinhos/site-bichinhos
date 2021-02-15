<template>
  <div class="container mx-auto px-4">
    <div class="hero flex flex-wrap items-center">
      <div
        class="w-full md:w-1/2 md:text-left text-center m-auto order-2 md:order-1"
      >
        <h1
          class="text-3xl md:text-4xl lg:text-5xl font-bold text-gray-800 mb-2"
        >
          O jeito mais fofinho de adotar seu bichinho
        </h1>
        <p class="text-lg text-gray-500 mb-6">
          Uma plataforma completa para proteger, adotar e encontrar bichinhos.
        </p>
        <button
          class="bg-primary border border-primary text-white px-6 py-2 rounded text-md font-medium whitespace-no-wrap hover:bg-primary-500"
        >
          Conhecer bichinhos
        </button>
      </div>
      <div
        class="w-full md:w-1/2 text-center md:text-left m-auto flex items-center justify-center order-2 md:order-1"
      >
        <img
          class=""
          src="@/assets/images/hero.svg"
          alt="Hero"
          style="max-width: 100%"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
.hero {
  height: calc(100vh - 80px);
}
</style>
