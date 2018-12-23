<template>
  <div class="row">
    <div class="column col-12">
      <div class="spacer"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Spacer"
};
</script>

<style lang="sass" scoped>
@import "../assets/sass/settings.sass"

.spacer
  height: 0.05555rem
  background-color: $spacer-c
  width: 100%
  margin: 100px 0
  position: relative
  z-index: 999

  
</style>
