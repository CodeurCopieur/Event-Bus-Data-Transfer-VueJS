<template>
  <form>
    <input type="text" placeholder="Search">
    <button type="submit" @click.prevent="">Search</button>
  </form>
</template>

<script>

export default {
  methods: {

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
        box-shadow: #3b49df 0px 1px 14px;
      }
    }
  }
</style>