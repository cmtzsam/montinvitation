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
    // let mm = gsap.matchMedia();

    // const copy_day = document.querySelector( '.Date--info h3.day' )
    // const copy_hour = document.querySelector( '.Date--info h3.hour' )
    // const copy_month = document.querySelector( '.Date--info .month' )
    // const copy_num = document.querySelector( '.Date--info .num' )
    // const flowers = document.querySelector('.Date--flowers img')
    // gsap.fromTo( copy_day, 
    //   { x: -50, opacity: 0 },
    //   { x: 0, opacity: 1, duration: .8  } 
    // );
    // gsap.fromTo( copy_hour, 
    //   { x: 50, opacity: 0 },
    //   { x: 0, opacity: 1, duration: .8  } 
    // );
    // gsap.fromTo( copy_month, 
    //   { y: -50, opacity: 0 },
    //   { y: 0, opacity: 1, duration: 1  } 
    // );
    // gsap.fromTo( copy_num, 
    //   { y: 50, opacity: 0 },
    //   { y: 0, opacity: 1, duration: 1  } 
    // );
    // gsap.fromTo( flowers, 
    //   { opacity: 0, scale: .8 },
    //   { opacity: 1, scale: 1, duration: 1  } 
    // );
    // gsap.to(copy_day, {
    //   x: 40,
    //   ease: "none",
    //   scrollTrigger: {
    //     markers: true,
    //     trigger: copy_day,
    //     scrub: true
    //   },
    // });
  }
}
</script>
<template>
  <section class="Date">
    <div class="o-container">

      <!-- <h2>Mi celebración</h2> -->
      <!-- <div class="Date--flowers flower-left">
        <img src="flower14.png" alt="Flores" class="img-full-responsive">
      </div>
      <div class="Date--flowers flower-right">
        <img src="flower15.png" alt="Flores" class="img-full-responsive">
      </div> -->
      <div class="Date--info">
        <div class="Date--data">
          <h3 class="day">Domingo</h3>
        </div>
        <div class="Date--day">
          <h4 class="month">OCT.</h4>
          <p class="num">01</p>
          <!-- <h6>2023</h6> -->
        </div>
        <div class="Date--data">
          <!-- <h3 class="hour">00:00 PM</h3> -->
          <h3 class="hour">04:44 PM</h3>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="sass">
@import './Date'
</style>