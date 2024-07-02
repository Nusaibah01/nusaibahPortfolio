<template>
    <div class="container">
     <div class="row">
        <h2 class="display-2" id="p">Testimonials</h2>
    </div>
        <div class="row gap-2 justify-content-center" v-if="myTestimonials">
          
            <Card v-for="(testimonial, id) in myTestimonials" :key="id">
                <template #cardHeader>
                    <h3>{{ testimonial.name}}</h3>
                    <img :src="testimonial.profile" :alt="testimonial.projectName" class="img-fluid" loading="lazy">
                </template>
                <template #cardBody>
                    <p>{{ testimonial.testimonial }} </p>
                
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