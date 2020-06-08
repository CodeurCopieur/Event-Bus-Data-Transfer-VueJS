<template>
  <div id="app">
    <Navigation></Navigation>
    <main>
      <div class="wrapper">
        <Article></Article>
      </div>
      
    </main>
    
  </div>
</template>

<script>

import Article from './assets/components/Article'
import Navigation from './assets/components/Navigation'

export default {
  name: 'app',
  components:{ Article, Navigation} ,
  data () {
    return {
      
    }
  }
}
</script>

<style lang="scss">

@import url('./assets/scss/index.scss');

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  header {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 10px 0px;
  }

  main {
    min-height: 80vh;
    display: flex;
    align-items: center;
    .wrapper {
      max-width: 80%;
      margin: 0 auto;
    }
  }
}
</style>
