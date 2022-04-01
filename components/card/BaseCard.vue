<template>
  <section
    v-for="card in cards"
    :key="card.id"
    class="grid text-center content-center bg-slate-400 shadow-lg shadow-slate-400 w-full max-w-[25vw] h-quarter bg-cover bg-center bg-no-repeat"
    :style="{ 'background-image': `url(${card.image.backgroundImage})` }"
  >
    <!-- <CardImage>{{ card.image }}</CardImage> -->
    <CardTitle>{{ card.title }}</CardTitle>
    <CardDescription>{{ card.description }}</CardDescription>
    <slot></slot>
  </section>
</template>

<script setup>
  const cards = [
    {
      title: "HTML",
      description: "Learn the foundational of web development",
      image: {
        backgroundImage:
          "https://images.unsplash.com/photo-1632882765546-1ee75f53becb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2232&q=80",
      },
    },
    {
      title: "CSS",
      description: "Learn how to style content of a webpage",
      image: {
        backgroundImage:
          "https://images.unsplash.com/photo-1472437774355-71ab6752b434?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1674&q=80",
      },
    },
    {
      title: "JavaScript",
      description: "Learn how to implement complex features to a website",
      image: {
        backgroundImage:
          "https://images.unsplash.com/photo-1579468118864-1b9ea3c0db4a?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2940&q=80",
      },
    },
  ];
</script>
