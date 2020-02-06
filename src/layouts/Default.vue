<template>

  <div class="layout">

    <div id="content-wrapper">

      <Header/>

      <slot/>
    
    </div>
    <Footer/>

  </div>




</template>

<script>
import Footer from '../components/Footer'
import Header from '../components/Header'

export default {
  components: {
    Footer,
    Header,
  },
}
</script>


<style lang="scss">

@import url("https://use.typekit.net/ahb6ubx.css");

body, html {
  height: 100%;
}

body {
  font-family: anonymous-pro, monospace !important  ;
  color: white !important;
  margin:0;
  padding:0;
  line-height: 1.5;
}

h1 {
font-family: nimbus-sans-extended, sans-serif;
font-style: normal;
font-weight: 900;
color: white;
font-size: 3rem;
}

.fade-enter-active {
  transition: margin-top 1s, opacity 1s;
}

.fade-enter {
  opacity: 0;
  margin-top: -100px;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100%;
  background-color: black;
}

#content-wrapper {
  flex: 1 0 auto;
  max-width: 1400px;
  width: 90vw;
  margin: 0 auto;
}
</style>
