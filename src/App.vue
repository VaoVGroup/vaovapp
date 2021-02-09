<template>
  <div id="app">
    <app-login></app-login>
  </div>
</template>

<script>
import Login from '../src/components/Login/Login'

export default {
  name: 'App',
  data() {
    return {
      
    }
  },
  methods: {
    
  },
  components: {
    "app-login" : Login
  }
 
}
</script>

<style>
</style>
