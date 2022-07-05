<template>
  <div id="app">
    <TheHeader id="Home"/>
    <TheJumbotron/>
    <TheServices id="Services"/>
    <TheAbout id="About"/>
    <TheProjects id="Projects"/>
    <TheResults id="Results"/>
    <TheContacts/>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import TheJumbotron from './components/TheJumbotron.vue';
import TheServices from './components/TheServices.vue';
import TheAbout from './components/TheAbout.vue';
import TheProjects from './components/TheProjects.vue';
import TheResults from './components/TheResults.vue';
import TheContacts from './components/TheContacts.vue';

export default {
  name: "App",
  components: { TheHeader, TheJumbotron, TheServices, TheAbout, TheProjects, TheResults, TheContacts },
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Montserrat&family=Poppins:wght@400;700;900&display=swap');
@import "~@fortawesome/fontawesome-free/css/all.min.css";

*{
  font-family: Montserrat;
}



</style>
