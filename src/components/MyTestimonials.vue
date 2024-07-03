<template>
    <div class="container">
     <div class="row">
        <h2 class="display-2" id="p">Testimonials</h2>
    </div>
        <div class="row gap-4 justify-content-center" v-if="myTestimonials">
<!-- <div class="testimonial-card">
  <div class="front">
    <img src="https://nusaibah01.github.io/all-images/images/Health Potion.gif" alt="Projects.gif">
  </div>
  <div class="back">
                       <img :src="testimonial.profile" :alt="testimonial.projectName" class="img-fluid d-inline" loading="lazy" id="back-image">
     <p>{{ testimonial.testimonial }} </p>
    
     <h5>{{ testimonial.name}}</h5>
  </div>
</div> -->
            <Card v-for="(testimonial, id) in myTestimonials" :key="id" class="card">
    
                <template #cardHeader>
                 
                    <img :src="testimonial.profile" :alt="testimonial.projectName" class="img-fluid d-inline" loading="lazy">
                    <hr>
                </template>
              
                <template #cardBody>
            
                    <h5>{{ testimonial.name}}</h5>
                    <hr>
                    <p>{{ testimonial.testimonial }} </p>
                        <hr>
                   
                </template>
            </Card> 
   
    

        </div>

        <Spinner v-else />
    </div>
</template>

<script setup>
import Card from './Card.vue'
import Spinner from "./Spinner.vue";
import { computed, onMounted } from "vue";
import { useStore } from "vuex";
  
  const store = useStore();
  const myTestimonials = computed(() => store.state. testimonials);
 
    onMounted(() => {
    store.dispatch("fetchTestimonials")
 
  })
</script>

<style scoped>
.card{
    background-color: black  !important;
    width: 18rem;
    aspect-ratio: 1 / 1;

    /* margin: 20px auto;
    position: relative;
    border: 1px solid;
    border-radius: 4px;
    transition: transform 2s;
    transform-style: preserve-3d; */

}
img{
    border: solid black;
    border-radius: 5px;
}
h2{
    font-family: "Press Start 2P", system-ui !important;
}

h5{
    color: tan;
    font-family: "Press Start 2P", system-ui;
     margin: 6px;
}
p{  

    margin: 30px;
    color: blue;
}
p:hover{
    color: red;
}
h2{
    margin: 30px;
}

</style>