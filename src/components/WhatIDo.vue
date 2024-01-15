<script setup>
  import { onMounted, ref } from 'vue'
  const curr_year = ref(new Date().getFullYear())
  const bg_music = ref('bg_music')
  onMounted(() => {
    console.log("Mounted, now time to play music!")
    // var audio = new Audio('/interstellar_nocopyright.mp3')
    // document.getElementById(bg_music.value).muted = "true"
    document.getElementById(bg_music.value).pause()
    document.getElementById(bg_music.value).play()

  })
  document.title = "Jeries Abedrabbo - What do I do?"
</script>

<template>

    <!-- Row for any alerts on top of page -->
    <div class="row">
      <div class="col">
        <!-- <div class="alert alert-danger">
          <strong>Problem!</strong> This is a placeholder for any new alers that might happen.
        </div>       -->
        <audio :id="bg_music" autoplay>
          <source src="/interstellar_nocopyright.mp3" type="audio/mpeg">
          <div class="alert alert-warning">
            <strong>Problem!</strong> Your browser does not support the audio element.
          </div>                
        </audio>        
      </div>
    </div>

    <!-- Main content -->
    <div class="row m-5">
      <div class="col-2">
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
      <div class="col-10 border-start border-2">
        <h1 class="w-100 text-danger" style="font-family:'Times New Roman'">What do I do?</h1>
        <p class="justify" style="font-family:'Times New Roman'; color: white;">
          I casually explore space lol jk. I worked for 5+ years as a Senior Software Engineer. Currently, I'm doing CubeSat
          development work. I'm also researching lunar effects on microalgae. Coool! isn't it?
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

    <!-- Footer content -->
    <div class="row fixed-bottom">
      <div class="col text-center">
        <small class="bg-primary text-warning">Copyright Reserved &copy; {{curr_year}} - Jeries Abedrabbo</small>
      </div>
    </div>

</template>

<style scoped>

</style>
