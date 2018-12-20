<template>
  <div class="content-holder">
    <ModalMenu/>
    <NavBar/>
  </div>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import ModalMenu from "../components/ModalMenu.vue";

export default {
  name: "Home",
  components: {
    NavBar,
    ModalMenu
  }
};
</script>

<style scoped lang="sass">
@import "../assets/sass/settings.sass"

</style>



