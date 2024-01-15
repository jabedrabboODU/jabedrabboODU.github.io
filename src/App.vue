<script setup>
  import { computed, ref } from 'vue'
  import PersonalPage from './components/PersonalPage.vue'
  import Studies from './components/Studies.vue'
  import WhatIDo from './components/WhatIDo.vue'
  import MyProjects from './components/MyProjects.vue'
  import UnderConstruction from './components/UnderConstruction.vue';
  import NotFound from './components/NotFound.vue'
  const u_constr = ref(true)

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

</script>

<template>
  <component :is="currentView" />
  <!-- <div v-if="u_constr" class="container-fluid"> -->
    <!-- <UnderConstruction v-if="u_constr" /> -->
  <!-- </div> -->
  <!-- <div v-else> -->
    <!-- <PersonalPage v-else /> -->
  <!-- </div> -->
</template>

<style>
body{
  background: url('/background.gif') fixed;
}
</style>
