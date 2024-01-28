<script setup>
  document.title = "Jeries Abedrabbo's Personal Website"
</script>

<template>
    <!-- Main content -->
    <div @click="playMusic" class="row m-5">
      <div class="row">
        <div class="col">
          <h1 class="text-center text-warning fw-bold" style="font-family:'Times New Roman'">Welcome to Jeries's Page!</h1>
        </div>
      </div>
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
        <h1 class="w-100 text-danger" style="font-family:'Times New Roman'">Who am I?</h1>
        <p class="justify" style="font-family:'Times New Roman'; color: white;">
          My name is Jeries Abedrabbo, and I'm a Senior Software Engineer and an Aerospace Engineer!
          <br>
          I'm interested in technology, computers, and SPACE! This webpage is a simple creation of mine to tell a little about myself.
          <br>
          As you can see, this page looks antique, but that's just the way I wanted it to be. The Internet in the late 1990s and early 2000s
          was a different beast. It was very cool to see all these cool webpages with colors all over the place, it gives me a warm sense
          of nostalgia, hence why I created this page to be like that. Well, I know you might not like it that way, but, ehh, it is what it is...
          <br>
          Please, be my guest, and take a look at the different sections of my personal website. Contact me if you need help, or if you want me to 
          help you with your next big idea, and if you have a million dollars you want to give me, this is an all inclusive offer.
          <br>
          Okay, enough talking! Dive in, pretty boy!
          <br>
          But before you go, please, have a coffee with me <img src="https://web.archive.org/web/20040715211000/http://www.geocities.com/two4dramma/cupsteamincoffee_tea.gif" alt="">  
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
