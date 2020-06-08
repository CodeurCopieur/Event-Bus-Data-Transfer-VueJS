<template>
  <header>
    <Logo></Logo>
    <Search></Search>
  </header>
  
</template>

<script>

import Logo from './Logo'
import Search from './Search'

export default {
  components:{Logo, Search}
}
</script>

<style lang="scss">
header {
  display: flex;
}

</style>