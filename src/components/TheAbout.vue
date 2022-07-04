<template>
  <div class="fluidcontainer">
    <div class="container h-100">
      <div class="row justify-content-center h-100">
        <div class="col h-100">
          <div
            class="div h-100 w-50 d-flex flex-column justify-content-center pe-5"
          >
            <h6 class="pb-4">ABOUT THE NETWORK</h6>
            <h2 class="pb-4">
              <span class="marked px-3 me-1">The</span>Company
            </h2>
            <p class="pb-5">
              For 12 years we have been providing audit and warranty, financial
              advice, risk advice, taxes and related services to select clients.
            </p>
            <div class="row card-container">
              <div
                class="col-lg-6 pb-5"
                v-for="skill in skills"
                :key="skill.title"
              >
                <h5 class="pb-3">
                  <i class="pe-3" :class="skill.icon"></i>{{ skill.title }}
                </h5>
                <p>{{ skill.paragraph }}</p>
              </div>
            </div>
            <div>
              <button type="button" class="btn btn-primary me-5">
                GET IN TOUCH
              </button>
              <button type="button" class="btn btn-outline-primary navelement">
                READ MORE
              </button>
            </div>
          </div>
        </div>
        <div class="col rightbg"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheAbout",
  components: {},
  data: function () {
    return {
      skills: [
        {
          title: "Tradition",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-medal",
        },
        {
          title: "Security",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-lock",
        },
        {
          title: "Certificate",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-regular fa-pen-to-square",
        },
        {
          title: "Expertise",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-graduation-cap",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

p {
  font-size: 1rem;
  color: lightgrey;
}

h2 {
  font-size: 3rem;
  color: white;
  .marked {
    color: white;
  }
}

h5 {
  font-family: Poppins;
  font-weight: 700;
  font-size: 1.5rem;
  color: white;
}

.btn-outline-primary{
 color: white;
}

.fluidcontainer {
  height: 850px;
  background-color: #111117;
}

.leftside {
  width: 50%;
}

.rightbg {
  background-image: url("../../public/images/about-4.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  width: 50%;
  height: 850px;
  position: absolute;
  right: 0;
}
</style>
