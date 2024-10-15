<template>
    <section id="graphic-projects" class="outline outline-1 outline-offset-0 outline-white py-16 px-4">
      <div class="container mx-auto text-gray-950">
        <h2 class="text-3xl font-bold text-center">Graphic Design</h2>
        <!-- Grid layout for graphic design projects -->
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 mt-8">
          <!-- Example Graphic Design Project -->
          <div class="flex flex-col p-6 rounded-lg shadow-md bg-gray-100">
            <h3 class="text-xl font-semibold">Logo Design</h3>
            <img
              src="/images/familytrip-1.png"
              alt="Logo Design"
              class="block mx-auto w-auto h-auto mt-4 rounded-lg shadow-md"
            />
            <p class="flex-grow mt-2 text-justify">
                This logo is a family trip logo and it embodies tradition and heritage with its earthy tones and the depiction of a classic stilt house. It tells a story of cultural roots, authentic charm, and timeless design.
            </p>
            <a
              href="#"
              class="hover:bg-gray-500 hover:text-gray-950 transition-colors duration-200 mt-4 inline-block bg-gray-800 text-white py-2 px-4 rounded-lg self-start"
              @click.prevent="openModal('/images/familytrip-1.png')"
            >View Design</a>
          </div>
  
          <!-- Another Graphic Design Project -->
          <div class="flex flex-col p-6 rounded-lg shadow-md bg-gray-100">
            <h3 class="text-xl font-semibold">Poster Design</h3>
            <img
              src="/images/unidentified-flying-whale-(UFW).png"
              alt="Poster Design"
              class="block mx-auto w-auto h-80 mt-4 rounded-lg shadow-md"
            />
            <p class="flex-grow mt-2 text-justify">
              A symbol of freedom and mystery, combining the serenity of the ocean with the infinite skies.
            </p>
            <a
              href="#"
              class="hover:bg-gray-500 hover:text-gray-950 transition-colors duration-200 mt-4 inline-block bg-gray-800 text-white py-2 px-4 rounded-lg self-start"
              @click.prevent="openModal('/images/unidentified-flying-whale-(UFW).png')"
            >View Design</a>
          </div>
        </div>
      </div>
  
      <!-- Modal for displaying large images -->
      <ImageModal :isVisible="isModalVisible" :imageSrc="selectedImage" @close="closeModal" />
    </section>
  </template>
  
  <script>
  import ImageModal from './ImageModal.vue';
  
  export default {
    name: 'GraphicProjects',
    components: {
      ImageModal,
    },
    data() {
      return {
        isModalVisible: false,
        selectedImage: '',
      };
    },
    methods: {
      openModal(imageSrc) {
        this.selectedImage = imageSrc;
        this.isModalVisible = true;
      },
      closeModal() {
        this.isModalVisible = false;
      },
    },
  };
  </script>
  
  <style scoped>
  section {
    background-color: rgb(209 213 219);
    padding: 4rem 0;
  }
  </style>
  