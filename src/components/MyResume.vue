<template>
    <div class="container">
      <div class="row">
        <h2 id="r">My Resume</h2>
      </div>
     
         <h3 id="edu">Education </h3>
        <div v-if="myEducation">
       <div class="timeline">
        <div class="holder left">
          <div class="content">
          <h3 v-for="(education, id) in myEducation" :key="id">{{ education.Year1 }}
          </h3>
          <hr>
         <img class="img-fluid" src=https://nusaibah01.github.io/all-images/images/lca.png loading="lazy" alt="LCA">
         <p  v-for="(education, id) in myEducation" :key="id">{{ education.School1}} </p>

          <p v-for="(education, id) in myEducation" :key="id">{{ education.Experiance1}}</p>
         <span class="left-a"></span>
       </div>
      </div>
      
        
     <div class="holder right">
      <div class="content">
      <h3 v-for="(education, id) in myEducation" :key="id">{{ education.Year2 }}</h3>
      <hr>
      <img class="img-fluid" src="https://nusaibah01.github.io/all-images/images/harvard.jpg" loading="lazy" alt="Harvard"> 
        <p v-for="(education, id) in myEducation" :key="id">{{ education.School2}} </p>
        <p v-for="(education, id) in myEducation" :key="id">{{ education.Experiance2}}</p>
   <span class="right-a"></span>
</div>
   </div>
   <div class="holder left">
    <div class="content">
    <h3 v-for="(education, id) in myEducation" :key="id">{{ education.Year3 }}</h3>
    <hr>
    <img class="img-fluid" src="https://nusaibah01.github.io/all-images/images/ka.png" loading="lazy" alt="ka">

        <p v-for="(education, id) in myEducation" :key="id">{{ education.School3}} </p>
        <p v-for="(education, id) in myEducation" :key="id">{{ education.Experiance3}}</p>  
  <span class="left-a"></span>
  </div>
  </div>
  </div>
  <div class="holder right">
    <div class="content">
      <h3 v-for="(education, id) in myEducation" :key="id">{{ education.Year4 }}</h3>   
      <hr>       
      <img class="img-fluid" src="https://nusaibah01.github.io/all-images/images/tlc.jpg" loading="lazy" alt="tlc">
    
      <p v-for="(education, id) in myEducation" :key="id">{{ education.School4}}</p>
        <p v-for="(education, id) in myEducation" :key="id">{{ education.Experiance4}}</p>

      <span class="right-a"></span>
      </div>
    </div>


        
       
      </div>
          <Spinner v-else />
        </div>
        
     
  
      
      <div class="row">
        
        <h2 id="s">Skills <i class="bi bi-briefcase-fill"></i></h2>
       
        <div>
            
            <h3>Personal Skill's</h3>
          <i class="bi bi-briefcase-fill"></i><p class="lead">Strong analytical and problem-solving abilities</p>
   
          <i class="bi bi-briefcase-fill"></i><p class="lead">Ability to work collaboratively in a team environment</p>
          <i class="bi bi-briefcase-fill"></i><p class="lead">Adaptability and willingness to learn new concepts</p>
          
          <h3 id="ts">Techical Skill's</h3>
        <!-- "techSkill1": "Html",--> 
  <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#E65100" d="M41,5H7l3,34l14,4l14-4L41,5L41,5z"/><path fill="#FF6D00" d="M24 8L24 39.9 35.2 36.7 37.7 8z"/><path fill="#FFF" d="M24,25v-4h8.6l-0.7,11.5L24,35.1v-4.2l4.1-1.4l0.3-4.5H24z M32.9,17l0.3-4H24v4H32.9z"/><path fill="#EEE" d="M24,30.9v4.2l-7.9-2.6L15.7,27h4l0.2,2.5L24,30.9z M19.1,17H24v-4h-9.1l0.7,12H24v-4h-4.6L19.1,17z" class="H"/></svg> 
        
      <!-- "techSkill2": "CSS" -->
<svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#0277BD" d="M41,5H7l3,34l14,4l14-4L41,5L41,5z"/><path fill="#039BE5" d="M24 8L24 39.9 35.2 36.7 37.7 8z"/><path fill="#FFF" d="M33.1 13L24 13 24 17 28.9 17 28.6 21 24 21 24 25 28.4 25 28.1 29.5 24 30.9 24 35.1 31.9 32.5 32.6 21 32.6 21z"/><path fill="#EEE" d="M24,13v4h-8.9l-0.3-4H24z M19.4,21l0.2,4H24v-4H19.4z M19.8,27h-4l0.3,5.5l7.9,2.6v-4.2l-4.1-1.4L19.8,27z" class="C"/></svg>

               
<!-- "techSkill3": "Bootstrap" -->
 <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#673ab7" d="M42,37c0,2.762-2.238,5-5,5H11c-2.761,0-5-2.238-5-5V11c0-2.762,2.239-5,5-5h26c2.762,0,5,2.238,5,5 V37z"/><path fill="#fff" d="M33.03,25.6c-0.65-0.9-1.59-1.52-2.8-1.85c0,0,1.02-0.37,1.94-1.75c0.55-0.88,0.83-1.94,0.83-3.18 c0-2.15-0.78-3.8-2.34-4.93C29.1,12.76,27.34,12,24.35,12H15v24h10.43c2.83-0.02,4.96-0.63,6.41-1.8c1.44-1.19,2.16-2.95,2.16-5.3 C34,27.6,33.68,26.5,33.03,25.6z M21,16c0,0,4.17,0,4.25,0c1.52,0,2.75,1.23,2.75,2.75c0,1.52-1.23,2.75-2.75,2.75 c-0.08,0-4.25,0-4.25,0V16z M26,32h-5v-6h5c1.66,0,3,1.34,3,3C29,30.66,27.66,32,26,32z" class="B"/></svg>
 
       <!-- "techSkill4": "JavaScript", -->
     
<svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><path fill="#ffd600" d="M6,42V6h36v36H6z"/><path fill="#000001" d="M29.538 32.947c.692 1.124 1.444 2.201 3.037 2.201 1.338 0 2.04-.665 2.04-1.585 0-1.101-.726-1.492-2.198-2.133l-.807-.344c-2.329-.988-3.878-2.226-3.878-4.841 0-2.41 1.845-4.244 4.728-4.244 2.053 0 3.528.711 4.592 2.573l-2.514 1.607c-.553-.988-1.151-1.377-2.078-1.377-.946 0-1.545.597-1.545 1.377 0 .964.6 1.354 1.985 1.951l.807.344C36.452 29.645 38 30.839 38 33.523 38 36.415 35.716 38 32.65 38c-2.999 0-4.702-1.505-5.65-3.368L29.538 32.947zM17.952 33.029c.506.906 1.275 1.603 2.381 1.603 1.058 0 1.667-.418 1.667-2.043V22h3.333v11.101c0 3.367-1.953 4.899-4.805 4.899-2.577 0-4.437-1.746-5.195-3.368L17.952 33.029z" class="Js"/></svg> 

<!-- "techSkill5": "VueJS" -->

<svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 48 48" width="100px" height="100px"><polygon fill="#81c784" points="23.987,17 18.734,8 2.974,8 23.987,44 45,8 29.24,8"/><polygon fill="#455a64" points="29.24,8 23.987,17 18.734,8 11.146,8 23.987,30 36.828,8" class="V"/></svg> 

       
     
   
        </div>
        <!-- <Spinner v-else /> -->
      </div>
  
     
    
  </template>
  
 <script setup>
 
  import Spinner from "./Spinner.vue";
  import { computed, onMounted } from "vue";
  import { useStore } from "vuex";
 
  
  const store = useStore();
  const myEducation = computed(() => store.state.education);
 
  // const mySkills = computed(() => store.state.skills);

    onMounted(() => {
    store.dispatch("fetchEducation")

    store.dispatch("fetchSkills")
  })

  </script>
  
  <style scoped>
h3, h2{
  /* margin: 30px; */
  font-family: "Press Start 2P", system-ui !important;
}
/* img{
  border-radius: 50%;
} */
svg:hover{
 
  border-color: solid white;
  gap: 60px;
  transform: scale(1);
  
}
svg{
top:-50px; 
left:-35px; 
 
z-index:999; 
cursor: pointer; 
/* -webkit-transition-property: all; 
-webkit-transition-duration: 0.3s; 
-webkit-transition-timing-function: ease;  */
} 
h3{
  color: tan;
}
/* .l {
  float: right;
}  */
  .EA{
    background-color:rgb(0, 255, 0);
    
    box-shadow: 10px 10px 20px rgb(0, 255, 0);

  }
  .A{
    box-shadow: 10px 10px 20px rgb(0, 255, 0);
  }
.G{
  box-shadow: 10px 10px 20px rgb(255, 204, 0);
}

.card{
  max-width: 100px;
}
#e-img{
 size: 3em;
}
#Edu{
  margin: 0 auto;
  text-align: center;
  
  margin: 0 auto;
  text-align: center;
  padding: 10px;
}

.holder p{
  font: bolder;
  font-family:  "Space Mono", monospace;
  color: white !important;
}
.timeline{
 max-width: 1200px;
  position: relative;
  margin: 100px auto;
}
.holder{
  padding: 10px 50px;
  position: relative;
  width: 50%;
  animation: movedown 1s linear forwards;
  opacity: 0;
}
@keyframes movedown{
0%{
  opacity: 1;
 transform: translateY(-30px);
}
100%{
  opacity: 1;
  transform: translateY(0px);
}
}
.hodler:nth-child(1){
  animation-delay: 0s;
}
.hodler:nth-child(2){
  animation-delay: 1s;
}
.hodler:nth-child(3){
  animation-delay: 2s;
}
.hodler:nth-child(4){
  animation-delay: 3s;
}

.content{
  padding: 20px 30px;
  background: #0C0C0C;
  position: relative;
  border-radius: 6px;
  font-size: 15px;
}
.left{
  left: 0;
}
.right{
  left: 50%;
}
.holder img{
  position: absolute;
  width: 40px;
  border-radius: 50%;
  right: -20px;
  top: 32px;
  z-index: 10;

}
.right img{
 left: -20px;
}
.timeline::after{
  content: '';
  position: absolute;
  width: 6px;
  height: 100%;
  background: black;
  top: 0;
  left: 50%;
  margin-left: -3px;
  z-index: -1;
  animation: moveline 6s linear forwards ;
}
@keyframes moveline{
  0%{
    height: 0;
  }
  100%{
    height: 100%;
  }
}
.content h3{
  font-weight: 400;
}
.content small{
  display: inline-block;
  margin-bottom: 15px;
}
.left-a{
  height: 0;
  width: 0;
  position: absolute;
  top: 28px;
  z-index: 1;
  border-top: 15px solid transparent;
  border-bottom: 15px solid transparent ;
  border-left: 15px solid white;
  right: -15px;
}
.right-a{
  height: 0;
  width: 0;
  position: absolute;
  top: 28px;
  z-index: 1;
  border-top: 15px solid transparent;
  border-bottom: 15px solid transparent ;
  border-right: 15px solid white;
  left: -15px;
}

@media screen and (max-width: 600px) {
  .timeline{
    margin: 50px auto;
}
.timeline::after{
  left: 31px;
}
.holder{
  width: 100%;
  padding: 80px;
  
}
}
#s, #ts{
  margin: 1em;
}
  </style>



