<template>
  <div class="app">
    <div class="container pt-5 pb-5">
      <h1 class="text-center">{{title}}</h1>
      <Navbar />
      <hr>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Navbar from './components/Navbar'
export default {
  name: 'app',
  components: {
    Navbar
  },
  data: () => ({
    title: 'Laravue'
  })
}
</script>
