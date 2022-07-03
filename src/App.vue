<template>
  <div id="app">
    <TheHeader/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';

export default {
  name: "App",
  components: {TheHeader,},
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Poppins:wght@400;700&display=swap');
@import "~@fortawesome/fontawesome-free/css/all.min.css";


</style>
