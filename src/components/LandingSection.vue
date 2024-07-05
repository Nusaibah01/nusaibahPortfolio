<template>
    <div class="container">
<div class="row vh-100 align-items-center">
    <div class="col">
        <img
          src="https://nusaibah01.github.io/all-images/images/20240422_101945.jpg"
          alt="logo"
          class="img-fluid w-75 shadow rounded-top border-top"
          loading="lazy"
        />
    </div>
    <div class="col">
        <div id="details">
            <h1 class="display-1" id="text">Nusaibah Charif</h1>
           <p v-if="title" id="title">
            
            <span> I am an {{ title}}</span>
        </p>
       <Spinner v-else />
        </div>
    </div>
</div>
    </div>
</template>

<script setup>
import Spinner from './Spinner.vue'
import { computed, onMounted, ref} from 'vue'
import  { useStore } from 'vuex'
const store =  useStore()
const jobTitle = computed(() => store.state.jobTitle)
const title = ref('Aspring Full Stack Developer')
const cnt = ref(-1)

function repeat() {
    try{
        if(cnt.value == jobTitle.value?.length) cnt.value = 0;
        title.value = jobTitle.value?.at(cnt.value)?.titel;
        setTimeout(repeat, 2000)
        cnt.value++
    } catch(e) {
        // 
    }
}
onMounted(() => {
store.dispatch('fetchJobTitle')
repeat()
})
</script>

<style scoped>
img{
    box-shadow: 10px 10px 20px 	rgb(210,180,140);
}
@media screen and (width < 800px) {
  #landing .row {
    display: block;
    height: auto;
  }
}
.text{
    color: white;
}
#title{
    color: yellow;
    font-family: "Press Start 2P", system-ui;
}
</style>
    