<template>
  <div id="app">
    <UserDashboard />
  </div>
</template>

<script>
import UserDashboard from '@/components/UserDashboard.vue'

export default {
  name: 'App',
  components: {
    UserDashboard
  }
}
</script>

<style>
@font-face {
  font-family: "Segoe";
  src: local("Fonts"),
   url(./fonts/segoe/SegoeUI.ttf) format("truetype");
} 
</style>