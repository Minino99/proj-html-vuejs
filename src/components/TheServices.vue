<template>
  <div class="services-container py-5">
    <div class="container py-5">
      <h6 class="pb-5">OUR BUSINESS AREAS</h6>
      <h2 class="pb-5">
        Excellence in<span class="marked px-3 mx-1">Services</span>
      </h2>
      <div class="d-flex justify-content-between align-items-center pb-5 gap-5">
        <p class="me-5">
          We are leaders in providing consultancy services with a set of
          cutting-edge technologies and a team of experienced and renowned
          professionals. These are some options that you can hire.
        </p>
        <button type="button" class="btn btn-primary ms-5">SEE ALL</button>
      </div>
      <div class="row">
        <div class="col-lg-4 col-md-6 p-0" v-for="service in services" :key="service.title">
          <div class="card p-5 m-3">
            <div class="card-body">
             <i class="pb-4" :class="service.icon"></i>
              <h5 class="card-title pb-4">{{service.title}}</h5>
              <p class="card-text">
                {{service.paragraph}}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheServices",
  components: {},
  data: function () {
    return {
      services: [
        {
          title: "Audit & Assurance",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-network-wired",
        },
        {
          title: "Financial Advisory",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-briefcase",
        },
        {
          title: "Analytics and M&A",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-chart-column",
        },
        {
          title: "Middle Marketing",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-plane",
        },
        {
          title: "Legal Consulting",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-globe",
        },
        {
          title: "Regulatory Risk",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          icon: "fa-solid fa-box",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

.services-container {
  width: 100%;
  height: fit-content;
  background-color: #eef4ed;
}

h2 {
  font-size: 3rem;
}

p {
  font-size: 1rem;
}

i{
 font-size: 3rem;
}

h5{
 font-family: Poppins;
 font-weight: 700;
 font-size: 1.5rem;
}

.card{
  background-color: #fff;
  border-radius: 10px;
  border-color: white;
  transition: transform 0.3s ease-in-out;

  &:hover{
    transform: translateY(-10px);
  }
}


</style>
