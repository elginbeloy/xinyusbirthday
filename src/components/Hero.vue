<template>
  <div class="hero">
    <a class="name">XINYU'S</a>
    <a class="birthday title">23RD</a>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Hero extends Vue {}
</script>

<style scoped lang="scss">
.hero {
  z-index: 0;
  position: absolute;
  width: 100%;
  height: 100%;
  background-image: url("../assets/background.jpg");
  background-position: center;
  background-attachment: fixed;
  background-size: cover;
  animation: highlight 1s infinite linear;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

@keyframes highlight {
  0%,
  99% {
    background-image: url("../assets/background.jpg");
  }
  50%,
  51% {
    background-image: url("../assets/background_two.jpg");
  }
}

.name {
  font-size: 48px;
  letter-spacing: 20px;
  color: #fff;
  text-shadow: 0 0 12px #ffffffa0;
  line-height: 48px;
}

.birthday {
  font-size: 112px;
  letter-spacing: 8px;
  color: #e56399;
  text-shadow: 0 0 12px #e56399a0;
}
</style>
