<template>
  <section id="about" class="py-16 px-4">
    <div class="container mx-auto text-gray-950">
      <h2 class="text-4xl font-bold text-center">About Me</h2>
      <p class="mt-6 text-lg text-center max-w-3xl mx-auto leading-relaxed">
        In the enchanted realm of Computer Science, I am a potion-brewing code wizard, 
        blending spells of software and mobile app development with the precision of a master alchemist. 
        My foundation is as steadfast as Hogwarts’ ancient walls, built upon a deep-seated passion for crafting magical tech solutions. 
        With a wand in hand and a heart full of creative curiosity, I approach every challenge with the problem-solving prowess of a true Gryffindor.
      </p>
      <p class="mt-6 text-lg text-center max-w-3xl mx-auto leading-relaxed">
        Driven by an unyielding quest for knowledge and a commitment to growth, 
        I seek opportunities in dynamic and growth-oriented environments where I can channel my technical expertise and bring a bit of wizardry to the world of technology.
      </p>
      <div class="mt-10 text-center">
        <h3 class="text-3xl font-semibold">Skills</h3>
        <ul class="list-none mt-4 inline-block max-w-3xl mx-auto leading-relaxed text-center space-y-2">
          <li class="text-lg">JavaScript, Vue.js, Python, Flutter, Dart, Ruby on Rails, HTML, CSS, Tailwind CSS, Google Firebase, Github, JSON</li>
          <li class="text-lg">Mobile Development, Agile, Problem Solving, Software Development, Creative Thinking,
            Team Player, Research and Analysis, Team Collaboration, Innovative Solutions.</li>
        </ul>
      </div>
      <div class="mt-12 text-center text-gray-100">
        <a 
          href="https://drive.google.com/uc?export=download&id=1TbgPmSrBXjVIkBem-MbsDwbhOW-lWPPm"
          class="hover:bg-gray-500 hover:text-gray-950 transition-colors duration-200 mt-8 inline-block bg-gray-800 text-white py-2 px-4 rounded-lg"
        >
          Download CV
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AboutMe',
};
</script>

<style scoped>
section {
  background-color: rgb(209 213 219);
  padding: 4rem 0;
}
a {
  color: inherit;
}
svg {
  transition: color 0.3s ease-in-out;
}
</style>
