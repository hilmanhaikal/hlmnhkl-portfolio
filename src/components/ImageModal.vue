<template>
  <div v-if="isVisible" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50">
    <div class="bg-white p-4 rounded-lg shadow-lg max-w-3xl max-h-[90vh] relative">
      <!-- Close Button -->
      <button
        @click="closeModal"
        class="absolute top-2 right-2 text-gray-600 hover:text-gray-900 text-lg font-bold"
      >
        &times;
      </button>

      <!-- Image in modal -->
      <img
        :src="imageSrc"
        alt="Design Preview"
        class="w-full h-auto object-contain max-h-[80vh] max-w-full"
      />
    </div>
  </div>
</template>

<script>
export default {
  name: 'ImageModal',
  props: {
    isVisible: Boolean,
    imageSrc: String,
  },
  methods: {
    closeModal() {
      this.$emit('close');
    },
  },
};
</script>

<style scoped>
/* Additional styles for responsive scaling */
</style>
