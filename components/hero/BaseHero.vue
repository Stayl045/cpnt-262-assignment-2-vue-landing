<template>
  <section
    v-for="hero in hero"
    :key="hero.id"
    :style="{ 'background-image': `url(${hero.image.backgroundImage})` }"
  >
    <HeroTitle>{{ mainHero.title }}</HeroTitle>
    <HeroDescription>{{ HeroDescription }}</HeroDescription>
  </section>
</template>

<script setup>
  import HeroTitle from "./HeroTitle.vue";

  const hero = [
    {
      title: "This is the best",
      description: "",
      image: {
        backgroundImage: "",
      },
    },
  ];
</script>
