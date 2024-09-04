<template>
  <header class="shadow-md py-4 bg-gray-900 text-white sticky top-0 z-50">
    <div class="container mx-auto flex items-center justify-between relative">
      <!-- Navbar icon on the left -->
      <div class="lg:hidden">
        <button @click="toggleMenu" class="focus:outline-none pl-2">
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

      <!-- "hlmnhkl" centered in the middle -->
      <h1 class="text-center text-2xl font-semibold absolute left-0 right-0 m-auto lg:static">hlmnhkl</h1>
      
      <!-- Empty div for spacing alignment -->
      <div class="lg:hidden"></div>

      <!-- Desktop navbar (optional) -->
      <nav class="hidden lg:flex lg:items-center lg:space-x-8">
        <ul class="flex space-x-8">
          <li><a href="#hero" class="hover:text-indigo-400 transition-colors duration-200 text-lg">Home</a></li>
          <li><a href="#projects" class="hover:text-indigo-400 transition-colors duration-200 text-lg">Projects</a></li>
          <li><a href="#about" class="hover:text-indigo-400 transition-colors duration-200 text-lg">About</a></li>
        </ul>
      </nav>
    </div>

    <!-- Overlay that closes the sidebar when clicked -->
    <div v-if="isMenuOpen" @click="closeMenu" class="fixed inset-0 bg-black bg-opacity-50 z-40 lg:hidden"></div>

    <!-- Side navbar for mobile -->
    <nav
      :class="{
        'translate-x-0': isMenuOpen,
        '-translate-x-full': !isMenuOpen
      }"
      class="fixed top-0 left-0 h-full bg-gray-900 w-64 transition-transform transform lg:hidden z-50"
    >
      <div class="px-6 py-4 bg-gray-800">
        <h1 class="text-2xl font-semibold text-white">hlmnhkl</h1>
      </div>

      <ul class="mt-6 flex flex-col space-y-6 pl-6">
        <li><a href="#hero" @click="closeMenu" class="hover:text-indigo-400 transition-colors duration-200 text-lg">Home</a></li>
        <li><a href="#projects" @click="closeMenu" class="hover:text-indigo-400 transition-colors duration-200 text-lg">Projects</a></li>
        <li><a href="#about" @click="closeMenu" class="hover:text-indigo-400 transition-colors duration-200 text-lg">About</a></li>
      </ul>
    </nav>
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
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
    closeMenu() {
      this.isMenuOpen = false;
    },
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

h1 {
  color: #ffffff;
  text-align: center;
}
</style>
