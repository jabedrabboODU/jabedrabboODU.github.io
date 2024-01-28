<script setup>
  import { computed, onMounted, ref } from 'vue'
  import PersonalPage from './components/PersonalPage.vue'
  import Studies from './components/Studies.vue'
  import WhatIDo from './components/WhatIDo.vue'
  import MyProjects from './components/MyProjects.vue'
  import UnderConstruction from './components/UnderConstruction.vue';
  import NotFound from './components/NotFound.vue'
  const u_constr = ref(false)

  const routes = {
  '/': u_constr.value ? UnderConstruction : PersonalPage,
  '/studies': Studies,
  '/whatido': WhatIDo,
  '/myprojects': MyProjects}

  const currentPath = ref(window.location.hash)

  window.addEventListener('hashchange', () => {
    currentPath.value = window.location.hash
  })

  const currentView = computed(() => {
    return routes[currentPath.value.slice(1) || '/'] || NotFound
  })

  const curr_year = ref(new Date().getFullYear())
  const email = ref('mailto:jeriesabedrabbo955@msn.com')
  const bg_music = ref('bg_music')
  onMounted(() => {
    console.log("Mounted, now time to play music!")
    // var audio = new Audio('/interstellar_nocopyright.mp3')
    // document.getElementById(bg_music.value).muted = "true"
    document.getElementById(bg_music.value).pause()
    if (u_constr.value) {
      console.log("We are not going to play music because we are under construction.")
    }
    else{
      document.getElementById(bg_music.value).play()
    }

  })
  
  function playMusic() {
    console.log("Playing now after click!")
    if(!u_constr.value){
      document.getElementById(bg_music.value).play()
    }
  }
</script>

<template>
  <!-- Row for any alerts on top of page -->
  <!-- Added w-100 to class row in this div, because it seems to remove the horizontal overflow scroll bar -->
  <div class="row mx-auto w-100">
    <div class="col mx-5">
      <!-- <div class="alert alert-danger">
        <strong>Problem!</strong> This is a placeholder for any new alers that might happen.
      </div>       -->
      <audio v-if="!u_constr" class="h-75" :id="bg_music" controls autoplay loop>
        <source src="/interstellar_nocopyright.mp3" type="audio/mpeg">
        <div class="alert alert-warning">
          <strong>Problem!</strong> Your browser does not support the audio element.
        </div>                
      </audio>        
    </div>
  </div>  
  <component :is="currentView" />
  <!-- Footer content -->
  <div class="row fixed-bottom">
    <div v-if="u_constr" class="row">
      <div class="col text-center">
        <small class="bg-white text-dark">Walking astronaut GIF created by: <a href="https://giphy.com/channel/Metarupx">Metarupx</a> Taken From: <a href="https://giphy.com/stickers/space-walking-astronaut-Vbh1DbykBFywj5VWY9">here</a></small>
      </div>
    </div>
    <div class="row">
      <div class="col text-center">
        <small class="bg-primary text-warning">Copyright Reserved &copy; {{curr_year}} - <a :href="email" class="text-warning">Jeries Abedrabbo</a></small>
      </div>
    </div>
  </div>
</template>

<style>
body{
  background: url('/background.gif') fixed;
}
</style>
