<template>
  <div id="app">
    <main>
      <nuxt/>
    </main>
  </div>
</template>

<style lang="scss">
@import '~@/assets/sass/_variables';

main {
  background: #fff;
  border-radius: 3px;
  border: 1px solid $primary-color;
  box-shadow: 3px 3px 0 $primary-color;
  display: flex;
  flex-direction: column;
  margin: 0 30px;
  width: 546px;
  padding: 40px 30px 30px;
  position: relative;
  transition: all 400ms;
  &:hover { box-shadow: 4px 4px 0 $primary-color }
  @include bp('xs') {
    margin: 0;
    padding: 25px;
    width: 100%;
  }
}
</style>

