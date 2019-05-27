<template>
  <ul class="nav justify-content-center">
    <li class="nav-item"><router-link to="/">Home</router-link></li>
    <li class="nav-item"><router-link to="/about">About</router-link></li>
  </ul>
</template>

<script>
export default {
  name: 'navbar'
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
