<template>
    <div class="container">
      <div class="row">
        <h1 id="r">My Resume</h1>
      </div>
  
      <div class="row">
        <h2 id="edu">Education<i class="bi bi-book-fill"></i></h2>
        <div v-if="myEducation">
        <img class="img-fluid" src=https://nusaibah01.github.io/all-images/images/lca.png loading="lazy" alt="LCA"><br>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.School1}}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Year1 }}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Experiance1}}</p>
        <img class="img-fluid" src="https://nusaibah01.github.io/all-images/images/harvard.jpg" loading="lazy" alt="Harvard"><br>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.School2}}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Year2 }}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Experiance2}}</p>
        <img class="img-fluid" src="https://nusaibah01.github.io/all-images/images/ka.png" loading="lazy" alt="ka"><br>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.School3}}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Year3 }}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Experiance3}}</p>
        <img class="img-fluid" src="https://nusaibah01.github.io/all-images/images/tlc.jpg" loading="lazy" alt="tlc">
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.School4}}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Year4 }}</p>
        <p class="lead" v-for="(education, id) in myEducation" :key="id">{{ education.Experiance4}}</p>
          
        
          
          

        </div>
        <Spinner v-else />
      </div>
  
      
      <div class="row">
        
        <h2>Skills <i class="bi bi-briefcase-fill"></i></h2>
       
        <div v-if="mySkills">
            
            <h3>Soft Skills</h3>
          <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.softSkill1 }}</p>
          <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.softSkill2 }}</p>
          <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.softSkill3 }}</p>
        <h3>Languages 
            <svg version="1.1" viewBox="0 0 1600 1600" width="30" height="30" xmlns="http://www.w3.org/2000/svg">
<path transform="translate(1053,266)" d="m0 0h271l23 1 22 4 19 7 16 9 12 9 10 9 8 8 9 12 10 17 9 24 3 15 1 8v148l-3 23-4 15-9 20-9 15-9 11-6 7-8 7-9 7-13 8-14 6-19 6-19 3-26 1h-330l-121 1h-31l-3-1 2-6 10-18 36-72 11-23 4-12 2-13v-118l2-22 5-22 10-23 9-15 8-10 9-10 15-12 21-12 14-6 16-4 8-1z" fill="#1C91F8"/>
<path transform="translate(972,799)" d="m0 0h298l51 1 25 1 18 2 16 5 16 8 12 7 14 11 13 13 11 16 10 19 6 18 3 14 1 9v146l-3 25-5 16-6 15-9 15-11 14-14 14-13 10-16 8-18 6-13 3-18 2-18 1-198 1h-74l-29-1-24-4-18-6-19-10-9-7-10-9-12-12-10-15-7-12-8-21-4-19-1-9v-127l-2-13-7-20-22-44-9-19-10-19-12-22-3-6v-4z" fill="#1C91F8"/>
<path transform="translate(467,1034)" d="m0 0h65l26 2 28 4 29 6 25 7 23 8 23 10 26 13 28 17 18 13 12 9 13 11 12 11 8 7 13 13 7 8 12 14 13 17 10 15 7 16 2 11v29l-1 52-4 4-4 1h-721l-5-5-1-79 2-13 8-16 7-11 11-14 9-11 13-14 1-2h2l2-4h2l2-4 12-12 8-7 8-8 8-7 18-14 14-10 20-12 16-9 22-11 20-8 22-8 25-7 36-7 31-4z" fill="#5F7A89"/>
<path transform="translate(482,467)" d="m0 0h33l28 3 23 5 15 5 20 9 20 11 16 11 10 8 12 11 17 17 11 14 10 15 10 18 8 17 12 36 4 18 2 18v32l-3 24-6 24-10 28-8 16-8 15-11 16-9 11-12 14-10 9-9 8-16 12-15 9-16 8-25 10-20 6-32 6-9 1h-30l-25-3-18-4-27-9-25-12-19-11-17-13-12-11-9-8-7-8-11-13-12-18-10-18-8-17-9-25-5-20-4-27v-31l6-36 7-25 8-19 8-16 9-16 12-16 12-14 19-19 11-9 10-8 18-11 16-8 24-10 24-6 21-3z" fill="#FDA531"/>
<path transform="translate(1168,332)" d="m0 0h16l10 4 8 9 8 16 11 29 15 49 7 25 7 21 9 32 10 28 9 29 3 12v7l-4 4-3 1h-33l-9-2-6-5-5-15-5-23-3-7v-3l-4-1-60 2-9 3-3 5-8 36-6 7-10 3-7 1h-32l-2-2v-8l5-19 6-16 18-60 13-44 30-90 8-17 4-5 6-4z" fill="#FDFDFD"/>
<path transform="translate(1161,865)" d="m0 0h11l8 4 8 9 1 2 1 15 12 3 7 1 64 2 10 2 3 4 2 7v17l-3 10-4 5-9 4-18 5-4 7-4 12-14 30-16 26-9 10-6 8-1 4 5 1 32 16 15 8 6 9 2 7-1 9-13 19-6 4-8-1-23-12-22-14-15-11-5-2-9 1-14 8-10 8-13 9-13 8-10 5h-7l-8-6-8-9-4-8-1-3v-8l6-9 12-9 21-10 10-5 9-7-4-6-9-9-8-7-5-6v-8l6-9 9-7 14-8h8l8 3 13 14 5 1 11-8 12-19 10-14 5-11 1-6-10-1-55-1h-83l-8-3-3-4-2-11 1-20 5-6 5-2 13-1 66-1 5-2 2-5-1-5v-8l3-6 8-5 6-3z" fill="#FDFDFD"/>
<path transform="translate(972,799)" d="m0 0h298l51 1 25 1 18 2 6 2v1l-10 1-23 1h-20l-22-1-9-1-33-1-90-1h-69l-41 1-17 1h-80l-18 1-8 1h-30l-36 2-7 1-6 3h-10l-5-5-2-5v-4z" fill="#147CE3"/>
<path transform="translate(1176,407)" d="m0 0 4 4 4 15 7 34 9 31 1 6-1 1-15 2h-12l-21-2-1-5 6-18 7-27 7-32 4-8z" fill="#1D92F9"/>
<path transform="translate(1333,658)" d="m0 0 23 1 6 1-3 3-15 2-26 1h-53l-346-1v-1l19-2 28-1 68-1h231l43-1h14z" fill="#0E7EED"/>
<path transform="translate(1324,1188)" d="m0 0h17l14 1 7 3-4 3-18 2-18 1-198 1h-74l-29-1-10-2v-1l44-2h132l38-1 28-1h18l31-2z" fill="#0D7DED"/>
<path transform="translate(1465,965)" d="m0 0h1v104l-1 11-2 2-1-7v-6l-1-4 1-13v-23l1-25 1-10z" fill="#0D7CEC"/>
<path transform="translate(1465,474)" d="m0 0h1v63l-2 13-2 2-1-7v-10l1-11v-16z" fill="#0D7CED"/>
</svg>
        </h3>
        <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.polyglotSkill1 }}</p>
        <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.polyglotSkill2 }}</p>
        <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.polyglotSkill3 }}</p>
        <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.polyglotSkill4 }}</p>
        
        <p class="lead" v-for="(skill, id) in mySkills" :key="id">{{ skill.polyglotSkill }}</p>
        
        <h3>Technical Skills</h3>
        <!-- "techSkill1": "Html",
      "techSkill2": "CSS",
      "techSkill3": "Bootstrap",
      "techSkill4": "JavaScript",
      "techSkill5": "VueJS" -->
      <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#E65100" d="M41,5H7l3,34l14,4l14-4L41,5L41,5z"/><path fill="#FF6D00" d="M24 8L24 39.9 35.2 36.7 37.7 8z"/><path fill="#FFF" d="M24,25v-4h8.6l-0.7,11.5L24,35.1v-4.2l4.1-1.4l0.3-4.5H24z M32.9,17l0.3-4H24v4H32.9z"/><path fill="#EEE" d="M24,30.9v4.2l-7.9-2.6L15.7,27h4l0.2,2.5L24,30.9z M19.1,17H24v-4h-9.1l0.7,12H24v-4h-4.6L19.1,17z"/></svg>
        
        <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#0277BD" d="M41,5H7l3,34l14,4l14-4L41,5L41,5z"/><path fill="#039BE5" d="M24 8L24 39.9 35.2 36.7 37.7 8z"/><path fill="#FFF" d="M33.1 13L24 13 24 17 28.9 17 28.6 21 24 21 24 25 28.4 25 28.1 29.5 24 30.9 24 35.1 31.9 32.5 32.6 21 32.6 21z"/><path fill="#EEE" d="M24,13v4h-8.9l-0.3-4H24z M19.4,21l0.2,4H24v-4H19.4z M19.8,27h-4l0.3,5.5l7.9,2.6v-4.2l-4.1-1.4L19.8,27z"/></svg>
       
        <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#673ab7" d="M42,37c0,2.762-2.238,5-5,5H11c-2.761,0-5-2.238-5-5V11c0-2.762,2.239-5,5-5h26c2.762,0,5,2.238,5,5 V37z"/><path fill="#fff" d="M33.03,25.6c-0.65-0.9-1.59-1.52-2.8-1.85c0,0,1.02-0.37,1.94-1.75c0.55-0.88,0.83-1.94,0.83-3.18 c0-2.15-0.78-3.8-2.34-4.93C29.1,12.76,27.34,12,24.35,12H15v24h10.43c2.83-0.02,4.96-0.63,6.41-1.8c1.44-1.19,2.16-2.95,2.16-5.3 C34,27.6,33.68,26.5,33.03,25.6z M21,16c0,0,4.17,0,4.25,0c1.52,0,2.75,1.23,2.75,2.75c0,1.52-1.23,2.75-2.75,2.75 c-0.08,0-4.25,0-4.25,0V16z M26,32h-5v-6h5c1.66,0,3,1.34,3,3C29,30.66,27.66,32,26,32z"/></svg>
    
        <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#ffd600" d="M6,42V6h36v36H6z"/><path fill="#000001" d="M29.538 32.947c.692 1.124 1.444 2.201 3.037 2.201 1.338 0 2.04-.665 2.04-1.585 0-1.101-.726-1.492-2.198-2.133l-.807-.344c-2.329-.988-3.878-2.226-3.878-4.841 0-2.41 1.845-4.244 4.728-4.244 2.053 0 3.528.711 4.592 2.573l-2.514 1.607c-.553-.988-1.151-1.377-2.078-1.377-.946 0-1.545.597-1.545 1.377 0 .964.6 1.354 1.985 1.951l.807.344C36.452 29.645 38 30.839 38 33.523 38 36.415 35.716 38 32.65 38c-2.999 0-4.702-1.505-5.65-3.368L29.538 32.947zM17.952 33.029c.506.906 1.275 1.603 2.381 1.603 1.058 0 1.667-.418 1.667-2.043V22h3.333v11.101c0 3.367-1.953 4.899-4.805 4.899-2.577 0-4.437-1.746-5.195-3.368L17.952 33.029z"/></svg>
       
        <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><polygon fill="#81c784" points="23.987,17 18.734,8 2.974,8 23.987,44 45,8 29.24,8"/><polygon fill="#455a64" points="29.24,8 23.987,17 18.734,8 11.146,8 23.987,30 36.828,8"/></svg>
  
   
        </div>
        <Spinner v-else />
      </div>
  
     
    </div>
  </template>
  
  <script setup>
  import Spinner from "./Spinner.vue";
  import { computed, onMounted } from "vue";
  import { useStore } from "vuex";
  
  const store = useStore();
  const myEducation = computed(() => store.state.education);
 
  const mySkills = computed(() => store.state.skills);

    onMounted(() => {
    store.dispatch("fetchEducation")

    store.dispatch("fetchSkills")
  })
  </script>
  
  <style scoped>

  </style>
  
