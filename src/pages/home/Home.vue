<template>
  <div>
    <home-header></home-header>
    <home-swriper></home-swriper>
  </div>
</template>

<script>
import HomeHeader from './components/Header'
import HomeSwriper from './components/Swriper'
export default {
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwriper
  }
}
</script>

<style>

</style>
