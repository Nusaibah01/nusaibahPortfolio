<template>
    <div class="container">
     <div class="row">
        <h2 class="display-2" id="p">My Projects</h2>
    </div>
        <div class="row gap-2 justify-content-center" v-if="myProjects">
          
            <Card v-for="(project, id) in myProjects" :key="id">
                <template #cardHeader>
                    <h3>{{ project.projectName }}</h3>
                    <img :src="project.image" :alt="project.projectName" class="img-fluid" loading="lazy">
                </template>
                <template #cardBody>
                    <p>{{ project.description }} </p>
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
h3{
    font-family: "Press Start 2P", system-ui;
    color: blanchedalmond;
}
p{
    font-family: "Space Mono", monospace;
    color: blue;
}
</style>