<template>
  <section
    v-for="card in cards"
    :key="card.id"
    class="grid bg-slate-400 shadow-lg shadow-slate-400 w-full max-w-[20vw] h-80 bg-cover bg-center bg-no-repeat hover:scale-105"
    :style="{ 'background-image': `url(${card.image.backgroundImage})` }"
  >
    <CardTitle>{{ card.title }}</CardTitle>
  </section>
</template>

<script setup>
  const cards = [
    {
      title: "Contemporary Designs",
      image: {
        backgroundImage:
          "https://images.unsplash.com/flagged/photo-1572392640988-ba48d1a74457?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1064&q=80",
      },
    },
    {
      title: "Modern Designs",
      image: {
        backgroundImage:
          "https://images.unsplash.com/photo-1501472312651-726afe119ff1?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=987&q=80",
      },
    },
    {
      title: "Stylistic Designs",
      image: {
        backgroundImage:
          "https://images.unsplash.com/photo-1484589065579-248aad0d8b13?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MjN8fGFydHxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=900&q=60",
      },
    },
    {
      title: "New Trendy Designs",
      image: {
        backgroundImage:
          "https://images.unsplash.com/photo-1571115764595-644a1f56a55c?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1041&q=80",
      },
    },
  ];
</script>
