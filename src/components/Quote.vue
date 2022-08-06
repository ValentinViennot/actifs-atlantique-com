<template>
  <div>
    <slot />
  </div>
</template>

<style lang="scss" scoped>
div {
  min-height: 200px;
  display: block;
  text-align: center;
  color: white;
  font-size: 3em;
  padding: 100px 0 100px 0;
  background: rgba($color: #000, $alpha: 0.3);
}
</style>