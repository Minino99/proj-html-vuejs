<template>
  <div class="header">
    <div class="container-fluid h-100">
      <div
        class="container h-100 d-flex justify-content-between align-items-center"
      >
        <div>
          <i class="fa-solid fa-clock"></i>
          Open Hours: Mon - Sat - 9:00 - 18:00
        </div>
        <div>
          <span class="px-3">
            <i class="fa-solid fa-phone"></i>
            +1 (305) 1234-5678
          </span>
          <span class="px-3">
            <i class="fa-solid fa-envelope"></i>
            hello@example.com
          </span>
          <span class="px-3">
            <i class="fa-brands fa-facebook-f"></i>
          </span>
          <span class="px-3">
            <i class="fa-brands fa-twitter"></i>
          </span>
          <span class="px-3">
            <i class="fa-brands fa-linkedin-in"></i>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheHeader",
  components: {},
};
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

.header {
  height: 5.5vh;
  color: $greytext;
}
.container-fluid {
  background-color: $bs-secondary;
  height: 100%;
}
</style>
