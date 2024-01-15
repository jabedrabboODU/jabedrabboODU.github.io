<script setup>
  import { ref } from 'vue'
  const curr_year = ref(new Date().getFullYear())
  const ss = ref('text-warning')
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
        <h1 :class="ss">Why you dooo diss!!??</h1>
        <img class="img-fluid w-50" style="object-fit:fill;" src="/again.gif" alt="Picture of man saying again, because you keep messing up and coming here.. sheesh! He's in space BTW">
      </div>
    </div>

    <!-- Footer content -->
    <div class="row fixed-bottom">
      <div class="col text-center">
        <small class="bg-primary text-warning">Copyright Reserved &copy; {{curr_year}} - Jeries Abedrabbo</small>
      </div>
    </div>

</template>

<style scoped>

</style>
