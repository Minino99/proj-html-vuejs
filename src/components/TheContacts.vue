<template>
<div class="container">
 <div class="row h-100 align-items-center">
  <div class="col-lg-8">
   <h6 class="pb-4">SEND A MESSAGE</h6>
       <h2 class=" pb-4">
      Get in<span class="marked px-3 mx-1">Touch</span>
    </h2>
    <p class="pb-5">We will respond to your message as soon as possible.</p>
    <div class="row pb-5 ps-3 justify-content-center">
     <div class="col-lg-6 p-4 ps-0 pb-0"><input class="form-control" type="text" placeholder="Name"></div>
     <div class="col-lg-6 p-4 ps-0 pb-0"><input class="form-control" type="text" placeholder="Email"></div>
     <div class="col-lg-6 p-4 ps-0 pb-0"><input class="form-control" type="text" placeholder="Phone"></div>
     <div class="col-lg-6 p-4 ps-0 pb-0"><input class="form-control" type="text" placeholder="More Info"></div>
     <div class="col-lg-12 p-4 ps-0 pb-0"><input class="form-control big" type="text" placeholder="Message"></div>
    </div>
     <div>
      <button class="btn btn-primary btn-block">SEND</button>
     </div>
  </div>
  <div class="col-lg-4">
   <h4 class="fw-bolder">Example Inc.</h4>
   <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
   <p>Praesent diam lacus, dapibus sed imperdiet consectetur.</p>
  </div>
 </div>
</div>
</template>

<script>
import {state} from "@/store";

export default{
 name: "TheContacts",
 components: {},
 data(){
  return {
   infos: state.infos,
  }
 },
 };

</script>

<style lang="scss" scoped>
@import "../assets/variables.scss";

.container{
 height: 800px;
}


.form-control::placeholder {

    color: #6c757d;
    opacity: 1;

}
.form-control::placeholder {

    color: #6c757d;
    opacity: 1;

} 
.form-control {
    display: block;
    width: 100%;
    padding: 0.75rem 0.75rem;
    font-size: 1rem;
    font-weight: 400;
    line-height: 1.5;
    color: #212529;
    background-color: lightgray;
    background-clip: padding-box;
    border: 1px solid #ced4da;
    -webkit-appearance: none;
    -moz-appearance: none;
    appearance: none;
    border-radius: 0.25rem;
    transition: border-color 0.15s ease-in-out, box-shadow 0.15s ease-in-out;
}

.big{
 padding-bottom: 10rem !important;
}

h2 {
  font-size: 3rem;
}


</style>