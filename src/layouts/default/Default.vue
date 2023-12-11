<template>
  <v-app>
    <default-bar />

    <default-view />
    <footer-component/>
  </v-app>
</template>

<script setup>
  import FooterComponent from '@/components/FooterComponent.vue';
  import DefaultBar from './AppBar.vue'
  import DefaultView from './View.vue'
</script>
