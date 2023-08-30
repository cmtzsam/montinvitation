<script>
import { gsap } from 'gsap';
import { ScrollTrigger } from 'gsap/dist/ScrollTrigger';
gsap.registerPlugin(ScrollTrigger);

export default {
  components: {
    gsap,
    ScrollTrigger,
  },
  mounted() { 
    const location_title = document.querySelector('.Location h2');
    const location_copy = document.querySelector('.Location--info');
    const location_flower1 = document.querySelector('.Location--flowers.left-flower');
    const location_flower2 = document.querySelector('.Location--flowers.right-flower');
    // gsap.fromTo( location_title, 
    //   { y: -50, opacity: 0 },
    //   { y: 0, opacity: 1, duration: .8  } 
    // );    
    // gsap.fromTo( location_copy, 
    //   { y: 50, opacity: 0 },
    //   { y: 0, opacity: 1, duration: .8  } 
    // ); 
    // gsap.fromTo( [location_flower1, location_flower2], 
    //   { y: 30, opacity: 0 },
    //   { y: 0, opacity: 1, duration: .6  } 
    // );        
  }
}
</script>
<template>
  <section class="Location">

    <div class="o-container">
      <!-- <h2>Ubicacion</h2> -->
      <div class="Location--flowers left-flower">
        <img src="http://codificarlos.com/pictures/flower14.png" alt="Flores" >
      </div>
      <div class="Location--flowers right-flower">
        <img src="http://codificarlos.com/pictures/flower17.png" alt="Flores" >
      </div>      
      <!-- <h3>THE GARDEN PAVILION THURSTFORD</h3> -->
      <div class="Location--info">
        <p>
          Crystal Plaza <br>
          305 W.Northfield Road <br>
          Livingston, NJ, 07039
        </p>
        <br>
        <button>
          &#9825; Ver mapa
        </button>
      </div>

    </div>

  </section>
</template>

<style lang="sass">
@import './Location'
</style>