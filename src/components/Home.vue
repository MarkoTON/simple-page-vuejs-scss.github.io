<template>
  <div class="home" >
    <Navbar />
    <Content />
    <Footer />
  </div>
</template>

<script>
import Navbar from './Navbar.vue'
import Content from './Content.vue'
import Footer from './Footer.vue'

export default {
  name: 'Home',
  components: {
    Navbar,
    Content,
    Footer
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss">
@include desktop {
  .container {
    width: 80%;
    margin: 0 auto;
    // background: red;
  }
}
</style>
