<script setup>
  import { ref } from 'vue'
  const curr_year = ref(new Date().getFullYear())
  document.title = "Jeries Abedrabbo - Under Construction!"
</script>

<template>

  <!-- Row for any alerts on top of page -->
  <div class="row">
    <div class="col">
      <!-- <div class="alert alert-danger">
        <strong>Problem!</strong> This is a placeholder for any new alers that might happen.
      </div>       -->
    </div>
  </div>

  <!-- Main content -->
  <div class="row text-center w-100">
    <div class="col">
      <img class="img-fluid" src="/jeries_walking.gif" alt="">
      <h4 style="color: chartreuse;">Ship is not working, Maintenance ongoing...</h4>
    </div>
  </div>

  <!-- Footer content -->
  <div class="row fixed-bottom">
    <div class="row">
      <div class="col text-center">
        <small class="bg-white text-dark">Walking astronaut GIF created by: <a href="https://giphy.com/channel/Metarupx">Metarupx</a> Taken From: <a href="https://giphy.com/stickers/space-walking-astronaut-Vbh1DbykBFywj5VWY9">here</a></small>
      </div>
    </div>
    <div class="row">
      <div class="col text-center">
        <small class="bg-primary text-warning">Copyright Reserved &copy; {{curr_year}} - Jeries Abedrabbo</small>

      </div>
    </div>
  </div>

</template>

<style scoped>

</style>
