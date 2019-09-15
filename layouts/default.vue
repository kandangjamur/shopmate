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
  @import url('https://fonts.googleapis.com/css?family=Playfair+Display:400,700&display=swap');

  body {
    font-family: 'Montserrat', sans-serif;
    color: #2e2e2e;
  }

  .font-playfair {
    font-family: 'Playfair Display', serif;
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

  .gray-3-color {
    color: #bababa;
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
    background: #f7f7f7;
  }

  .grey-2-bg {
    background: #efefef;
  }
</style>
