<template>
  <div class="turing-app">
    <Header />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/header'
import Footer from '@/components/footer'
export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Montserrat:300,400,500,600,700&display=swap');

  body {
    font-family: 'Montserrat', sans-serif;
    color: #2e2e2e;
  }

  .wrapper {
    width: 95%;
    margin: auto;
  }

  /* color */
  .red-color {
    color: #e9425c;
  }

  .gray-color {
    color: #969696;
  }

  .gray-2-color {
    color: #6c6c6c;
  }

  /* background */
  .red-bg {
    background: #e9425c;
  }

  .black-bg {
    background: #2e2e2e;
  }

  .gray-bg {
    background: #969696;
  }

  .grey-bg {
    background: #f2f2f2;
  }
</style>
