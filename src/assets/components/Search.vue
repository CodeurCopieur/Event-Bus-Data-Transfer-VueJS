<template>
  <form>
    <input type="text" placeholder="Search" v-model="value" >
    <button type="submit" @click.prevent="emitSearchValue">Search</button>
  </form>
</template>

<script>

import { EventBus } from './../../main'

export default {
  data (){
    return {
      value: '',
    }
  },
  methods: {
    
    emitSearchValue() {
      EventBus.$emit('search', this.value)
      console.log(this.value);

    }
  }

}
</script>

<style lang="scss">
  form {
    input {
      outline: none;
    }
    button {
      border: none;
      outline: none;
      background: #3b49df;
      color: #fff;
      padding: 5px;
      cursor: pointer;
      font-size: 15px;
      text-transform: uppercase;
      transition: all 380ms ease-in-out;

      &:hover {
        box-shadow: #3b49df 3px 3px 3px;
      }
    }
  }
</style>