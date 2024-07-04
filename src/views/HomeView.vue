<template>
  <div class="container">
   <div class="row">
    
    <section class="row" id="landing">
      <LandingSection/>
    </section>

    <section class="row" id="about">
<About/>
    </section>
    <section class="row" id="resume">
     <MyResume/>
    </section>
    <section class="row" id="project">
   <MyProjects/>
    </section>
    <section class="row" id="testimonials">
   <MyTestimonials/>
    </section>
    <section class="row" id="reachMe">
    <ContactMe/>
    </section>
   </div>
  </div>
</template>

<script>

import LandingSection from '@/components/LandingSection.vue';
import About from '@/components/AboutMe.vue';
import MyResume from '@/components/MyResume.vue';
import MyProjects from '@/components/MyProjects.vue';
import MyTestimonials from '@/components/MyTestimonials.vue';
import ContactMe from '@/components/ContactMe.vue'
export default {
  name: 'HomeView',
components: {
 LandingSection,
  About,
  MyResume, 
  MyProjects,
  MyTestimonials,
  ContactMe
  

}
   }

</script>
