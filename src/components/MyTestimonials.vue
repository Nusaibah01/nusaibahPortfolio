<template>
    <div class="container">
     <div class="row">
        <h2 class="display-2" id="p">Testimonials</h2>
    </div>
        <div class="row gap-6 justify-content-center" v-if="myTestimonials">

            <Card v-for="(testimonial, id) in myTestimonials" :key="id" class="card">
    
                <template #cardHeader>
                 
                    <img :src="testimonial.profile" :alt="testimonial.name" class="img-fluid d-inline" loading="lazy">
                    <hr>
                </template>
              
                <template #cardBody>
            
                    <h5>{{ testimonial.name}}</h5>
                    <hr>
                    <p>{{ testimonial.testimonial }} </p>
                    <small> {{testimonial.role }}</small>
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
    font-family: "Space Mono", monospace; 

    color: white;
}
p:hover{
    color: red;
}
h2{
    margin: 30px;
}
small{
    font-family: "Space Mono", monospace;
    color: tan;
}
.testimonial-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 20px; /* Adjust as needed */
}

.testimonial-card {
  flex: 1 1 calc(50% - 10px); /* Two cards per row initially */
  max-width: calc(50% - 10px);
  padding: 20px;
  background-color: #f9f9f9;
  border: 1px solid #ccc;
  text-align: center;
}

@media (min-width: 768px) {
  .testimonial-card {
    flex-basis: calc(33.33% - 20px); /* Three cards per row on larger screens */
    max-width: calc(33.33% - 20px);
  }
}

@media (max-width: 767px) {
 
    .testimonial-card, h2 {
    flex-basis: calc(50% - 20px); /* Two cards per row on smaller screens */
    max-width: calc(50% - 20px);
  }
}

</style>