<script setup>
  document.title = "Jeries Abedrabbo - My Projects"
</script>

<template>

    <!-- Main content -->
    <div @click="playMusic" class="row m-5">
      <div class="col-md-2">
        <div class="row">
          <div class="col">
            <img class="img-fluid" style="border-style: inset; border-width: 4px; border-color: yellow; " src="/me.jpg" alt="A Picture of me, myself, and I">
          </div>
        </div>
        <div class="row">
          <div class="col text-center">
            <strong style="color: aqua;">
              Handsome me at the cosmosphere museum Hutchinson, KS
            </strong>
          </div>
        </div>
      </div>
      <div class="col-md-10 border-start border-2">
        <h1 class="w-100 text-danger" style="font-family:'Times New Roman'">Projects of mine:</h1>
        <p class="justify" style="font-family:'Times New Roman'; color: white;">
          I'll add them later. Don't worry!
        </p>
        <ul>
          <li style="list-style-image: url('/favicons/icons8-comet-emoji-favicons12/Web/icons8-comet-emoji-16.png')">
            <a  href="#/studies">What have I studied?</a>
          </li>
          <li style="list-style-image: url('/favicons/icons8-person-astronaut-emoji-favicons19/Web/icons8-person-astronaut-emoji-16.png');">
            <a  href="#/whatido">What do I do?</a>
          </li>
          <li style="list-style-image: url('/favicons/icons8-venus-planet-color-favicons14/Web/icons8-venus-planet-color-16.png');">
            <a href="#/myprojects">Some projects of mine <img src="/ezgif.com-resize.gif" alt="fire GIF" ></a>
          </li>   
          <li style="list-style-image: url('/earth.gif');">
            <a href="/">Back to earth?</a>
          </li>             
        </ul>
        <!-- <div class="row">
          <div class="col">
            <li style="list-style-image: url('/favicons/icons8-comet-emoji-favicons12/Web/icons8-comet-emoji-16.png')">
              <a  href="#">What have I studied?</a>
            </li>
          </div>
        </div>
        <div class="row">
          <div class="col">
            <li style="list-style-image: url('/favicons/icons8-person-astronaut-emoji-favicons19/Web/icons8-person-astronaut-emoji-16.png');">
              <a  href="#">What do I do?</a>
            </li>
          </div>
        </div>
        <div class="row">
          <div class="col">
            <li style="list-style-image: url('/favicons/icons8-venus-planet-color-favicons14/Web/icons8-venus-planet-color-16.png');">
              <a href="#">Some projects of mine <img src="/ezgif.com-resize.gif" alt="fire GIF" ></a>
            </li>
          </div>
        </div> -->
      </div>
    </div>

</template>

<style scoped>

</style>
