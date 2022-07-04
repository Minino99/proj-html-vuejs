<template>
  <div class="container py-5 my-5" id="categories">
    <h6 class="text-center pt-5 pb-4">WE DO MORE FOR EVERYONE</h6>
    <h2 class="text-center pb-5">
      Actions &<span class="marked px-3 mx-1">Projects</span>
    </h2>
    <div class="d-flex justify-content-center gap-5 pb-5">
      <span v-for="category in categories" :key="category"
        ><a href="#categories">{{ category.toLocaleUpperCase() }}</a></span
      >
    </div>
    <div class="row">
      <div
        class="col-lg-4 col-md-6 mb-4"
        v-for="project in projects"
        :key="project.title"
      >
        <div class="card bg-dark text-white overflow-hidden">
          <img :src="`images/project${project.img}.jpg`" class="card-img" />
            <div class="card-img-overlay d-flex flex-column justify-content-end">
             <div class="align-self-end arrow pb-5 px-3"><i class="fa-solid fa-arrow-right arrow"></i></div>
              <h5 class="card-title text-center pb-4">{{ project.title }}</h5>
              <p class="card-text text-center">
                {{ project.paragraph }}
              </p>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheProjects",
  components: {},
  data: function () {
    return {
      categories: [
        "all",
        "institutional",
        "social",
        "events",
        "innovation",
        "environment",
        "technology",
      ],
      projects: [
        {
          title: "Academic professional program in social media",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          img: "-1",
        },
        {
          title: "President's speech at the annual meeting",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          img: "-2",
        },
        {
          title: "International business trip in Shanghai",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          img: "-3",
        },
        {
          title: "Technology workshop with education theme",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          img: "-4",
        },
        {
          title: "Donation of clothes and food to the partner NGO",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          img: "-5",
        },
        {
          title: "Confraternization of the procurement team",
          paragraph: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          img: "-6",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

h2 {
  font-size: 3rem;
}

h5 {
  font-family: Poppins;
  font-weight: 700;
  font-size: 1.5rem;
  color: white;
}

.card {
  border-radius: 15px;
  border-color: white;
}

.arrow{
 color:white;
 font-size: 2rem;
 transform: translateY(-100%);
 opacity: 0;
 transition: opacity 0.3s;
}

  .card:hover .card-text{
   display: block;
   transform: translateY(0);
   opacity: 1;
  }

    .card:hover .card-title{
   transform: translateY(0);
  }

  
    .card:hover .card-img{
   transform: scale(1.2);
  filter: brightness(0.5) blur(5px);
  }

  .card:hover .arrow{
   opacity: 1;
  }

.row{
 transform: scale(0.8);
}


.col {
  padding: 0;
}

.card-title{
 transform: translateY(90%);
 transition: transform 0.3s;
}

.card-text{
 transform: translateY(100%);
 opacity: 0;
 transition: opacity 0.3s, transform 0.3s;
}

.card-img {
  filter: brightness(0.5);
  transition: transform 0.3s, filter 0.3s;
}

</style>
