<template>
  <div class="app">
    <div class="container pt-5 pb-5">
      <h1 class="text-center">Laravue</h1>
      <ul class="nav justify-content-center">
        <li class="nav-item">
          <router-link to="/">Home</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/about">About</router-link>
        </li>
      </ul>
      <hr>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'
import BootstrapVue from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

Vue.use(BootstrapVue)

export default {
  name: 'app'
}
</script>

<style lang="scss" scoped>
.nav {
  position: relative;
  .nav-item {
    border-right: 1px solid #DDD;
    padding: 0 0.5rem;
    &:last-child {
      border-right: none;
    }
  }
}
</style>