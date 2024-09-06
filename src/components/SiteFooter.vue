<template>
  <footer class="text-gray-100 text-center py-4">
    <div class="container mx-auto text-center">
      <p>&copy; 2024 Hilman Haikal. All rights reserved.</p>
      <div class="space-x-4 pt-1">
          <a href="https://linkedin.com/in/hilmanhaikal" class="hover:text-gray-500 transition-colors duration-200">linkedin</a>
          <a href="https://github.com/hilmanhaikal" class="hover:text-gray-500 transition-colors duration-200">Github</a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'SiteFooter',
};
</script>

<style scoped>
footer {
  background-color: rgb(3 7 18);
  color: white;
  text-align: center;
  padding: 1rem;
}
</style>
