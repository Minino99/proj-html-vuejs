<template>
  <div id="app">
    <TheHeader/>
    <TheJumbotron/>
    <TheServices/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheJumbotron from './components/TheJumbotron.vue';
import TheServices from './components/TheServices.vue';

export default {
  name: "App",
  components: { TheHeader, TheJumbotron, TheServices },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Poppins:wght@400;700;900&display=swap');
@import "~@fortawesome/fontawesome-free/css/all.min.css";

*{
  font-family: Montserrat;
}



</style>
