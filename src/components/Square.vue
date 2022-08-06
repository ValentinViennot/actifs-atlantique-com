<script setup lang="ts">
defineProps({
  title: { type: String, required: true },
  description: { type: String },
});
</script>


<template>
  <a class="tile" :id="title" :href="'#'+title">
    <div class="letter">{{ title.substr(0, 1) }}</div>
    <div class="details">
      <div class="title">{{ title }}</div>
      <div class="info">{{ description }}</div>
    </div>
  </a>
</template>

<style lang="scss" scoped>
a.tile {
  background-color: var(--vt-c-indigo);
  color: whitesmoke;
  width: 12%;
  max-width: 250px;
  min-width: 180px;
  height: 200px;
  max-width: 100%;
  margin: auto;
  display: inline-block;
  margin: 10px;
  text-align: left;
  overflow: hidden;
  border-radius: 3px;
  box-shadow: 0 0 20px 0 rgba(0, 0, 0, 0.05);
  position: relative;
  text-decoration: none;

  &::before {
    content: "";
    background: linear-gradient(
      to bottom,
      rgba(0, 0, 0, 0) 0,
      rgba(0, 0, 0, 0.7) 100%
    );
    width: 100%;
    height: 100%;
    opacity: 0;
    top: 100%;
    position: absolute;
    left: 0;
    z-index: 1;
    transition-property: top, opacity;
    transition-duration: 0.3s;
  }

  &:hover,
  &:focus {
    background-color: var(--vt-c-orange);
    &::before {
      top: 0%;
      opacity: 1;
    }

    div.details {
      div.title,
      div.info {
        opacity: 1;
        top: 0;
      }
    }
  }

  > div.letter {
    display: block;
    text-align: center;
    width: 100%;
    height: 100%;
    font-size: 140px;
  }

  div.details {
    z-index: 2;
    padding: 20px;
    position: absolute;
    bottom: 0;
    top: 0;
    left: 0;
    right: 0;
    color: #fff;
    font-size: 16px;

    div {
      display: block;
      position: relative;
      transition-property: top, opacity;
      transition-duration: 0.3s;
    }

    div.title {
      top: 150px;
      line-height: 1;
      font-weight: 600;
      font-size: 20px;
      transition-delay: 0s;
    }
    div.info {
      top: 200px;
      opacity: 0;
      line-height: 1.2;
      margin-top: 5px;
      font-size: 18px;
      transition-timing-function: ease-in-out;
    }
  }
}
</style>