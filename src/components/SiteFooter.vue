<template>
  <footer class="text-gray-100 text-center py-4">
    <div class="container mx-auto text-center">
      <p>&copy; 2024 Hilman Haikal. All rights reserved.</p>
      <div class="space-x-2 pt-2">
        <i class="fa fa-linkedin-square" style="font-size:24px"></i>
        <a href="https://linkedin.com/in/hilmanhaikal" class="hover:text-gray-500 transition-colors duration-200 pr-2">linkedin</a>
        <i class="fa fa-github-square" style="font-size:24px"></i>
        <a href="https://github.com/hilmanhaikal" class="hover:text-gray-500 transition-colors duration-200 pr-2">Github</a>
        <i class="fa fa-envelope-square" style="font-size:24px"></i>
        <a href="mailto: hilmanhaikal7@gmail.com" class="hover:text-gray-500 transition-colors duration-200 pr-2">Hilman Haikal</a>
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
