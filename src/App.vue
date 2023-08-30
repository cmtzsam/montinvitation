<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <!-- <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header> -->

  <RouterView />
</template>

<style lang="sass">
/* amatic-sc-regular - latin */
@font-face 
  font-display: swap 
  font-family: 'Amatic SC'
  font-style: normal
  font-weight: 400
  src: url('./fonts/amatic-sc-v26-latin-regular.woff2') format('woff2') 

/* amatic-sc-700 - latin */
@font-face 
  font-display: swap 
  font-family: 'Amatic SC'
  font-style: normal
  font-weight: 700
  src: url('./fonts/amatic-sc-v26-latin-700.woff2') format('woff2') 

/* herr-von-muellerhoff-regular - latin */
@font-face
  font-display: swap
  font-family: 'Herr Von Muellerhoff'
  font-style: normal
  font-weight: 400
  src: url('./fonts/herr-von-muellerhoff-v21-latin-regular.woff2') format('woff2') 

@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: normal
  font-weight: 400
  src: url('./fonts/cormorant-v21-latin-regular.woff2') format('woff2') 


@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: italic
  font-weight: 400
  src: url('./fonts/cormorant-v21-latin-italic.woff2') format('woff2') 


@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: normal
  font-weight: 500
  src: url('./fonts/cormorant-v21-latin-500.woff2') format('woff2') 


@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: italic
  font-weight: 500
  src: url('./fonts/cormorant-v21-latin-500italic.woff2') format('woff2') 


@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: normal
  font-weight: 600
  src: url('./fonts/cormorant-v21-latin-600.woff2') format('woff2') 


@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: italic
  font-weight: 600
  src: url('./fonts/cormorant-v21-latin-600italic.woff2') format('woff2') 


@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: normal
  font-weight: 700
  src: url('./fonts/cormorant-v21-latin-700.woff2') format('woff2') 


@font-face 
  font-display: swap 
  font-family: 'Cormorant'
  font-style: italic
  font-weight: 700
  src: url('./fonts/cormorant-v21-latin-700italic.woff2') format('woff2') 

</style>
