<script setup>
import Banner from '../components/Banner.vue'
import Date from '../components/Date.vue';
import Location from '../components/Location.vue';
import Dresscode from '../components/Dresscode.vue';
import Invitation from '../components/Invitation.vue';
</script>

<template>
  <main>
    <Banner />
    <Date />
    <Location />
    <Dresscode />
    <Invitation />
  </main>
</template>

<style lang="sass">
@import "@/assets/custom/mainstyle.sass"
</style>