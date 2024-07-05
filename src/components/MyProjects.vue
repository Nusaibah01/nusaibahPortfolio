<template>
    <div class="container">
     <div class="row">
        <h2 id="p">My Projects</h2>
    </div>
        <div class="row gap-2 justify-content-center d-flex align-items-stretch" v-if="myProjects">
          
            <Card v-for="(project, id) in myProjects" :key="id" class="card">
                <template #cardHeader>
                    <h5 class="d-inline">{{ project.projectName }}</h5>
                    <hr>
                    <div>
                   <img :src="project.image" :alt="project.projectName">
                    <hr>
                </div>
                    <!-- <img :src="project.image" :alt="project.projectName" class="img-fluid" loading="lazy"> -->
                </template>
                <template #cardBody>
                    <p>{{ project.description }} </p>
                    <hr>
                  <a :href="project.github" target="_blank">
                    <button><i class="bi bi-github"></i></button></a>
                    <a :href="project.vercel" target="_blank">
                    <button><i class="bi bi-triangle-fill"></i></button>
                </a>
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
  const myProjects = computed(() => store.state.projects);
 


    onMounted(() => {
    store.dispatch("fetchProjects")

 
  })

</script>

<style scoped>

h5{
    font-family: "Press Start 2P", system-ui;
    color: tan;
}
p{
    font-family: "Space Mono", monospace;
    color: white;
}
p:hover{
    color: yellow;
}
img{
    object-fit: contain;
    aspect-ratio: 1/1;
    width: 150px;
    height: 130px;
}
/* img{
    margin: 3px;
    padding: 0;
    width: 48px;
    height: 48px;
} */
button{
    border-radius: 3px;
    background-color: white;
    margin-bottom: 30px;
}
.container{
    background-color: black;
}
.card{
    background-color: #0C0C0C ;
    
}
h2{
    margin: 1em;
    font-family: "Press Start 2P", system-ui !important;
    color: white !important;
  
}
i{
    background-color: white;
}
/* Projects */
#p{
  font-family: "Space Mono", monospace;
  color: silver;
}
</style>