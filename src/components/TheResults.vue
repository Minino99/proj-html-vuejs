<template>
  <div>
    <div
      class="numbers-container align-items-center d-flex flex-column justify-content-center"
    >
      <h6 class="pb-4">WHAT ARE WE DOING</h6>
      <h2 class="pb-5">
        <span class="marked px-3 me-1">Results</span> in Numbers
      </h2>
      <div class="container d-flex justify-content-around">
        <div v-for="data in datas" :key="data.description">
          <h4 class="text-center">{{ data.number }}</h4>
          <h5>{{ data.description }}</h5>
        </div>
      </div>
    </div>
    <div class="partners">
      <div class="container"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheResults",
  components: {},
  data: function () {
    return {
      datas: [
        {
          number: "128",
          description: "Certifications",
        },
        {
          number: "230",
          description: "Employees",
        },
        {
          number: "517",
          description: "Customers",
        },
        {
          number: "94",
          description: "Countries Served",
        },
      ],
      partners: [
        {
          name: "Woo Commerce",
          logo: "-1",
        },
        {
          name: "WordPress",
          logo: "-2",
        },
        {
          name: "pingdom",
          logo: "-3",
        },
        {
          name: "jQuery",
          logo: "-4",
        },
        {
          name: "less",
          logo: "-5",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

.numbers-container {
  height: 600px;
  background-image: url("../../public/images/bg-7.jpg");
  background-size: cover;
  background-attachment: fixed;
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

h4 {
  font-family: Poppins;
  font-weight: 700;
  font-size: 2.4rem;
  color: #00a6a6;
}

.partners {
  background-color: #111117;
  height: 300px;
}
</style>
