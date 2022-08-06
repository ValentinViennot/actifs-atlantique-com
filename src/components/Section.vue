<template>
  <div class="bloc">
    <slot />
  </div>
</template>

<style lang="scss" scoped>
div.bloc {
  display: flex;
  vertical-align: middle;
  background: white;
  min-height: 200px;
  padding: 40px;
}
</style>