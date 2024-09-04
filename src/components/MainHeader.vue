<template>
  <header class="shadow-md py-4 bg-gray-900 text-white sticky top-0 z-50">
    <div class="container mx-auto flex flex-wrap items-center justify-between">
      <h1 class="pl-2 tracking-wide text-2xl font-semibold">hlmnhkl</h1>
      <div class="lg:hidden">
        <button @click="isMenuOpen = !isMenuOpen" class="focus:outline-none pr-1">
          <svg
            :class="{ 'transform rotate-90': isMenuOpen }"
            class="w-8 h-8 transition-transform duration-300 ease-in-out"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
          </svg>
        </button>
      </div>
      <nav
        :class="{
          'translate-x-0': isMenuOpen,
          '-translate-x-full': !isMenuOpen
        }"
        class="fixed top-0 left-0 h-full bg-gray-900 w-64 transition-transform transform lg:hidden z-40"
      >
        <ul class="mt-24 flex flex-col space-y-6 pl-6">
          <li><a href="#hero" @click="isMenuOpen = false" class="hover:text-indigo-400 transition-colors duration-200 text-lg">Home</a></li>
          <li><a href="#projects" @click="isMenuOpen = false" class="hover:text-indigo-400 transition-colors duration-200 text-lg">Projects</a></li>
          <li><a href="#about" @click="isMenuOpen = false" class="hover:text-indigo-400 transition-colors duration-200 text-lg">About</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'MainHeader',
  data() {
    return {
      isMenuOpen: false,
    };
  },
};
</script>

<style scoped>
header {
  background-color: #1f2937;
}

a {
  color: #e5e7eb;
}

a:hover {
  color: #6366f1;
}

nav {
  background-color: #1f2937;
}
</style>
