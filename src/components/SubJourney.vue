<template>
  <div class="row">
    <div class="column col-8 responsive-12">
      <h1>{{title}}</h1>
      <p>{{content}}</p>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: "SubJourney",
  props: ["title", "content"]
};
</script>


<style lang="sass" scoped>
@import "../assets/sass/settings.sass"

.row
    padding-bottom: 100px

h1
    margin-bottom: 20px
    font: 
      weight: 600
      size: 2rem

ul
  columns: 2

li
  margin-bottom: 10px
  font-weight: 600

p
  margin-bottom: 30px
</style>