<template>
  <section
    v-for="hero in hero"
    :key="hero.id"
    :style="{ 'background-image': `url(${hero.image.backgroundImage})` }"
    class="h-screen bg-cover"
  >
    <TheBaseHeader />
    <div class="grid text-center content-center mt-64">
      <SmallTitle>{{ hero.smltitle }}</SmallTitle>
      <!-- <HeroDescription>{{ hero.description }}</HeroDescription> -->
      <HeroTitle>{{ hero.title }}</HeroTitle>
      <CardButton
        ><button
          class="text-white p-7 border rounded-2xl mt-6 font-extrabold hover:bg-slate-50 hover:text-black xs:invisible md:visible"
        >
          {{ hero.button }}
        </button></CardButton
      >
    </div>
  </section>
</template>

<script setup>
  const hero = [
    {
      smltitle: "Stephan Taylor",
      title: "Design that is equal part tasteful, equal part pretentious",
      description: "This is the worst",
      image: {
        backgroundImage:
          "https://images.unsplash.com/photo-1519681393784-d120267933ba?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2070&q=80",
      },
      button: "START YOUR DESIGN",
    },
  ];
</script>
