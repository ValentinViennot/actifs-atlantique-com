<template>
  <Section>
    <div class="squares_bloc">
      <slot />
    </div>
  </Section>
</template>

<style lang="scss" scoped>
div.squares_bloc {
  display: block;
  margin: auto;
  text-align: center;
  align-self: center;
}
</style>