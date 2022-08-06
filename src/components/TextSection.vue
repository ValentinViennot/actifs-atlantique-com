<template>
  <Section class="text_bloc">
    <slot />
  </Section>
</template>

<style lang="scss">
div.text_bloc {
  flex-direction: column;
  > p {
    font-size: 1.3em;
    margin-top: 20px;
    &.bold {
      font-weight: bold;
    }
  }
  > h2 {
    font-size: 1.9em;
    font-weight: bold;
  }
}
</style>