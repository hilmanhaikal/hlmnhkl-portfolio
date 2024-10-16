<template>
  <section id="projects" class="outline outline-1 outline-offset-0 outline-white py-16 px-4">
    <div class="container mx-auto text-gray-950">
      <h2 class="text-3xl font-bold text-center">Projects</h2>
      <!-- Update grid classes for responsive layout -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8 mt-8">
        <!-- Example Project -->
        <div class="flex flex-col p-6 rounded-lg shadow-md bg-gray-100">
          <h3 class="text-xl font-semibold">MindGuard</h3>
          <img
            src="/images/project1.png"
            alt="MindGuard Project"
            class="block mx-auto w-auto h-auto mt-4 rounded-lg shadow-md"
          />
          <p class="flex-grow mt-2 text-justify">
            The MindGuard project is a web-based mental health assessment tool using machine learning models for PHQ-9 depression severity analysis and sentiment analysis, built with Python, Flask, and supporting libraries like nltk, scikit-learn, and Seaborn.
          </p>
          <a
            href="https://github.com/hilmanhaikal/MindGuard"
            class="hover:bg-gray-500 hover:text-gray-950 transition-colors duration-200 mt-4 inline-block bg-gray-800 text-white py-2 px-4 rounded-lg self-start"
            target="_blank"
            rel="noopener noreferrer"
          >View Project</a>
        </div>
        <!-- Recipe App -->
        <div class="flex flex-col p-6 rounded-lg shadow-md bg-gray-100">
          <h3 class="text-xl font-semibold">Recipe App</h3>
          <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-2">
            <img
              src="/images/project2 (1).png"
              alt="RecipeApp"
              class="block mx-auto w-60 h-auto mt-4 rounded-lg shadow-md"
            />
            <img
              src="/images/project2 (2).png"
              alt="RecipeApp"
              class="block mx-auto w-60 h-auto mt-4 rounded-lg shadow-md"
            />
            <img
              src="/images/project2 (3).png"
              alt="RecipeApp"
              class="block mx-auto w-60 h-auto mt-4 rounded-lg shadow-md"
            />
          </div>
          <p class="flex-grow mt-2 text-justify">
            The Recipe App is a Flutter-based mobile application that allows users to browse, manage, and store recipes with detailed instructions and images, using JSON as the data source.
          </p>
          <a
            href="https://github.com/hilmanhaikal/recipe_app"
            class="hover:bg-gray-500 hover:text-gray-950 transition-colors duration-200 mt-4 inline-block bg-gray-800 text-white py-2 px-4 rounded-lg self-start"
            target="_blank"
            rel="noopener noreferrer"
          >View Project</a>
        </div>
        <!-- Laptop Cost Estimation -->
        <div class="flex flex-col p-6 rounded-lg shadow-md bg-gray-100">
          <h3 class="text-xl font-semibold">Laptop Cost Estimation</h3>
          <img
            src="/images/project3 (1).png"
            alt="LaptopCostEstimation"
            class="block mx-auto w-auto h-auto mt-4 rounded-lg shadow-md"
          />
          <p class="flex-grow mt-2 text-justify">
            The project is a Cost Estimation application, using technologies such as Python, Flask, and scikit-learn. Key features include a machine learning model for price prediction, a web interface for user interaction, and necessary configuration files for deployment.
          </p>
          <a
            href="https://github.com/hilmanhaikal/Cost-estimation"
            class="hover:bg-gray-500 hover:text-gray-950 transition-colors duration-200 mt-4 inline-block bg-gray-800 text-white py-2 px-4 rounded-lg self-start"
            target="_blank"
            rel="noopener noreferrer"
          >View Project</a>
        </div>
        <div class="flex flex-col p-6 rounded-lg shadow-md bg-gray-100">
          <h3 class="text-xl font-semibold">Login Page Template</h3>
          <img
            src="/images/login.png"
            alt="LaptopCostEstimation"
            class="block mx-auto w-auto h-auto mt-4 rounded-lg shadow-md"
          />
          <p class="flex-grow mt-2 text-justify">
            The project is a simple login page template.
          </p>
        </div>
        <div class="flex flex-col p-6 rounded-lg shadow-md bg-gray-100">
          <h3 class="text-xl font-semibold">E-Commerce Home Page Template</h3>
          <img
            src="/images/homepage.png"
            alt="LaptopCostEstimation"
            class="block mx-auto w-auto h-auto mt-4 rounded-lg shadow-md"
          />
          <p class="flex-grow mt-2 text-justify">
            This e-commerce homepage template showcases a sleek shoe store design with a hero image of a beige sneaker. The navigation bar includes links to Home, Products, About, and Contact, plus a shopping cart icon. The main section highlights four shoe options, each with an image, name, price, and Add to Cart button for easy shopping.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'ProjectList',
};
</script>

<style scoped>
section {
  background-color: rgb(209 213 219);
  padding: 4rem 0;
}
</style>
