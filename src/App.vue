<template>
  <div id="app">
    <Home/>
  </div>
</template>

<script>
import Home from './components/Home'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>
<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0px;
  font-family: 'Open Sans';
}
</style>
