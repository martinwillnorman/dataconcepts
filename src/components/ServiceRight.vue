<template>
  <div class="row right">
    <div class="column col-7 responsive-12">
      <div class="content-wrapper">
        <h1 class="section-header left medium">{{title}}</h1>
        <p>{{content}}</p>
        <slot></slot>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ServiceRight",
  props: ["title", "content"]
};
</script>


<style lang="sass" scoped>
@import "../assets/sass/settings.sass"

.content-wrapper
  padding-bottom: 100px

ul
  columns: 2

li
  margin-bottom: 10px
  font-weight: 600

p
  margin-bottom: 30px
</style>
