<template>
  <div id="particles">
      <div class="container-fluid d-flex flex-column">
        <div
          class="container d-flex justify-content-between align-items-center p-3 nav-container"
        >
          <div class="h-100">
            <img
              src="../../public/images/logo.png"
              class="h-100"
              alt=""
              srcset=""
            />
          </div>
          <div class="navelements d-flex align-items-center">
            <span
              v-for="navelement in navElements"
              :key="navelement.name"
              class="px-4 navelement"
              >{{ navelement.name.toUpperCase() }}</span
            >
            <button type="button" class="btn btn-primary navelement">
              GET IN TOUCH
            </button>
          </div>
        </div>
        <div
          class="align-self-center d-flex flex-column justify-content-center h-100 jumbotitle"
        >
          <h1 class="bigtitle text-center pb-3">
            Ready<span class="marked px-3 ms-2">Team</span>
          </h1>
          <p class="pb-5 text-center" style="max-width: 500px;">
            No matter what your company needs, we will be ready to assist you in
            the best possible way.
          </p>
          <div class="d-flex justify-content-center gap-4">
            <div>
              <button type="button" class="btn btn-primary">
                GET IN TOUCH
              </button>
            </div>
            <button type="button" class="btn btn-outline-primary navelement">
              READ MORE
            </button>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheJumbotron",
  components: {},
  data: function () {
    return {
      navElements: [
        {
          name: "Home",
          link: "",
        },
        {
          name: "Services",
          link: "",
        },
        {
          name: "About",
          link: "",
        },
        {
          name: "Projects",
          link: "",
        },
        {
          name: "Results",
          link: "",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

.container-fluid {
  height: 94.5vh;
  background-image: url("../../public/images/bg-parallax.png");
  background-position: center;
}

.nav-container {
  height: 70px;
}

.navelement {
  font-size: 1.1rem;
}

.bigtitle {
  font-size: 4.7rem;
  font-weight: 900;
  color: $bs-secondary;
}


#particles{
 background-image: url("../../public/images/particles.png");
}
</style>
