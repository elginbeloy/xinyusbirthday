<template>
  <div class="tocome">
    <img src="@/assets/decoration.svg" class="decoration" />

    <a class="title">Included</a>
    <div class="body">
      First is the one and only, Charlotte Tilbury. Not the person, but ya know
      she signed off. Hopefully you haven't had/seen these before, and you like
      what you find.
    </div>
    <div class="image-container">
      <img src="@/assets/present_1.jpeg" />
      <img src="@/assets/present_2.jpg" />
    </div>
    <div class="body">
      The second is intangible now, but potentially worth a much more later. I
      guess it's up to you and how you want to use it 😉
    </div>
    <a class="elgin-bucks">
      10 Elgin Bucks
    </a>
    <div class="body">
      and counting... Redemable for any favor ... any favor ... any ... favor.
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class ToCome extends Vue {}
</script>

<style scoped lang="scss">
.tocome {
  position: absolute;
  top: 100%;
  width: 100%;
  height: auto;
  padding: 140px 40px;
  box-shadow: 0 -48px 48px #000000c0;
  background: #000;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
}

.decoration {
  position: absolute;
  right: 0;
  top: calc(50% - 300px);
  width: 300px;
  height: 600px;
  animation: highlight 1s infinite linear;
}

@keyframes highlight {
  0%,
  100% {
    opacity: 1;
  }
  30%,
  80% {
    opacity: 0;
  }
}

.title {
  max-width: 600px;
  font-size: 48px;
  letter-spacing: 6px;
  color: #fff;
  text-shadow: 0 0 12px #ffffffa0;
  line-height: 128px;
}

.body {
  max-width: 600px;
  font-size: 18px;
  line-height: 36px;
  color: #fff;
}

.image-container {
  position: relative;
  margin-top: 20px;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  margin-bottom: 60px;

  img {
    height: 300px;
    margin-right: 20px;
    border-radius: 8px;
    box-shadow: 0 0 8px #ffffffa0;
  }
}

.elgin-bucks {
  margin-top: 40px;
  margin-bottom: 40px;
  text-decoration: capitalize;
  font-size: 48px;
  color: #fff;
  letter-spacing: 8px;
  line-height: 48px;
  text-shadow: 0 0 12px #e56399;
}
</style>
