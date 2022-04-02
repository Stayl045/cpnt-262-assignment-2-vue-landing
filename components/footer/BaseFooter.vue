<template>
  <section
    class="grid grid-cols-3 bg-black opacity-95 h-96 mt-7 text-white w-full"
  >
    <FooterCopyright>
      <footer>
        <p>&copy; Stephan Taylor</p>
      </footer>
    </FooterCopyright>
    <div class="grid col-start-5 pt-14 pr-12">
      <FooterSocialMedia>
        <a :href="'/'" class="hover:text-red-400 text-3xl">Social</a>
        <a :href="'/'" class="hover:text-red-400">Instagram</a>
        <a :href="'/'" class="hover:text-red-400">FaceBook</a>
        <a :href="'/'" class="hover:text-red-400">YouTube</a>
      </FooterSocialMedia>
    </div>
  </section>
</template>
