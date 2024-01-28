<script setup>
  import { ref } from 'vue'
  const lost_text = ref('text-warning')
  document.title = "404 Not Found!"
</script>

<template>

    <!-- Row for any alerts on top of page -->
    <div class="row">
      <div class="col">
        <div class="alert alert-primary">
          <strong>Uh oh!</strong> 404 Page Not Found :(
        </div>             
      </div>
    </div>

    <!-- Main content -->
    <div class="row text-center my-5">
      <div class="col">
        <h1 :class="lost_text">Lost in space?</h1>
        <img class="img-fluid w-50" style="object-fit:fill;" src="/again.gif" alt="Picture of man saying again, because you keep messing up and coming here.. sheesh! He's in space BTW">
      </div>
    </div>
</template>

<style scoped>

</style>
