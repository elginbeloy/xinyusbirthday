<template>
  <div class="home">
    <Hero />
    <ToCome />
  </div>
</template>

<script>
import Hero from "@/components/Hero.vue";
import ToCome from "@/components/ToCome.vue";

export default {
  name: "Home",
  components: {
    Hero,
    ToCome
  }
};
</script>
