<template>
  <v-container class="fill-height app-container fadeIn makeWider">
    <v-responsive class="align-center text-center fill-height">

      <v-img class="imageHeight" :max-height="getImageHeight()" src="@/assets/art12.png" />

      <div class="py-2" />
      <AnimatedHeader />
      <div class="text-body-2 font-weight-light mb-n1 font-italic coolColor">Coming soon...</div>
      
      <div class="py-4" />
      
      <!-- <AnimatedTitle class="custom-font" /> -->
      <div class="container">
    <div class="row">
      <div class="col-md-12 text-center">
          <h2 class="text-h3  mb-n0 makeSmaller">Tauriform</h2>
      </div>
    </div>
  </div>
      <!-- <h1 class="text-h3  custom-font makeSmaller">Tauriform</h1> -->
      <br>
    
      

      <div class="py-3" />


      <v-row class="d-flex align-center justify-center">
        <v-col cols="auto">
          <p>Incorporating advanced extraterrestrial techniques, Tauriform crafts intricate sonic landscapes that transport listeners to intergalactic realms. <br>Hailing from the cosmic frontier, Tauriform's signature chunky bass tones resonate powerfully, even shaking the vacuum of outer space.</p>
    
          
        </v-col>
      </v-row>
      <v-row class="d-flex align-center justify-center">


        <v-col cols="auto">
          <v-btn
            href="https://soundcloud.com/tauriform-music"
            min-width="164"
            rel="noopener noreferrer"
            target="_blank"
            variant="text"
            class="prettyColor"
          >
            <v-icon
              icon="mdi-soundcloud"
              size="large"
              start
            />

            Soundcloud
          </v-btn>

          <v-btn
            href="https://duckduckgo.com/"
            min-width="164"
            rel="noopener noreferrer"
            target="_blank"
            variant="text"
            class="prettyColor2"
          >
            <v-icon
              icon="mdi-spotify"
              size="large"
              start
            />

            Spotify
          </v-btn>

          
      
          <div class="py-8" /> 
          <div class="py-11 help" /> 
          <div class="py-11 help" /> 
          <div class="py-10 help" /> 
        </v-col>
     


      </v-row>
    </v-responsive>
  </v-container>
</template>

<script lang="ts" setup>
  import AnimatedHeader from '../components/AnimatedHeader.vue';
  import AnimatedTitle from '../components/AnimatedHeaderTitle.vue'
import { onMounted } from 'vue';
  import { ref } from 'vue';

const getImageHeight = () => {
  return window.innerWidth > 900 ? 450 : 300;
};

import { gsap } from "gsap";
  
  const tl = gsap.timeline({ repeat: -1 });
  tl.to(".title", 30, { backgroundPosition: "-960px 0" });

</script>


<style scoped>

@import '../fonts/custom-font.css';



.custom-font {
  letter-spacing: 0.1em !important;
font-family: 'CustomFont' !important;



/* Add other styling as needed */
}
.app-container {
  background-image: url('@/assets/bgTauriform.png'); 
  background-size: cover; 
  background-position: center; 
  /* height: 100vh;  */
  /* width: 100%; */
  /* display: flex; */
  /* justify-content: space-around; */
  align-items: center;
  color: white; 

}

.fadeIn {
  opacity: 0;
  animation: fadeIn 3s forwards;
}


@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.coolColor {
  color: #ffadcb;
}

.prettyColor {
  /* color: #F98057; */
  color: #ffadcb;
}

.prettyColor2 {
  /* color: #5cf957; */
  color: #ffadcb;
}

@media screen and (max-width: 600px) {
  .makeSmaller {
    font-size: 2em !important; /* Adjust the font size for small screens */
  }
}

.imageHeight {
  height: 400 !important;
}

@media screen and (min-width: 1260px) {
  .help {
    display: none;
  }
}

@media (min-width: 400px ) {
  .v-container {
    max-width: 100% !important;
}
}

@keyframes lights {
    0% {
        color: hsl(230, 40%, 80%);
        text-shadow:
            0 0 0.75em hsla(298, 100%, 50%, 0.075),
            0 0 0.075em hsla(320, 100%, 60%, 0.3),
            -0.5em -0.075em 0.15em hsla(212, 100%, 60%, 0),
            0.5em 0.075em 0.15em hsla(234, 100%, 60%, 0);
    }

    30% {
        color: hsla(230, 80%, 90%, 0.692);
        text-shadow:
            0 0 0.75em hsla(293, 100%, 50%, 0.274),
            0 0 0.075em hsla(298, 100%, 60%, 0.301),
            -0.25em -0.075em 0.125em hsla(199, 100%, 60%, 0.2),
            0.25em 0.075em 0.125em hsla(200, 100%, 60%, 0.4);
    }

    40% {
        color: hsla(226, 100%, 95%, 0.589);
        text-shadow:
            0 0 0.75em hsla(305, 100%, 50%, 0.267),
            0 0 0.075em hsla(320, 100%, 90%, 0.5),
            -0.125em -0.075em 0.075em hsla(204, 100%, 60%, 0.2),
            0.125em 0.075em 0.075em hsla(200, 100%, 60%, 0.4);
    }

    70% {
        color: hsla(230, 80%, 90%, 0.795);
        text-shadow:
            0 0 0.75em hsla(295, 100%, 55%, 0.192),
            0 0 0.075em hsla(184, 100%, 55%, 0.5),
            0.25em -0.075em 0.125em hsla(226, 100%, 60%, 0.2),
            -0.25em 0.075em 0.125em hsla(200, 100%, 54%, 0.4);
    }

    100% {
        color: hsl(230, 40%, 80%);
        text-shadow:
            0 0 0.75em hsla(180, 4%, 36%, 0.2),
            0 0 0.075em hsl(300, 76%, 45%),
            0.5em -0.075em 0.15em hsla(239, 100%, 60%, 0),
            -0.5em 0.075em 0.15em hsla(200, 100%, 60%, 0);
    }
}

  
  
  h2 {
    margin: auto;
    font-family: 'CustomFont' !important;
    /* font-size: 3.5rem; */
    /* font-weight: 300; */
    animation: lights 5s 750ms linear infinite;
    /* font-family: 'CustomFont', sans-serif; */
  
  }

  h1 {
    margin: auto;
    font-family: 'CustomFont' !important;
    /* font-size: 3.5rem; */
    /* font-weight: 300; */
    animation: lights 5s 750ms linear infinite;
    /* font-family: 'CustomFont', sans-serif; */
  
  }


</style>