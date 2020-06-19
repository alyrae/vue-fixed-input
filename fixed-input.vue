<template>
  <input type="text" @blur="blur">
</template>
<script>
export default {
  data() {
    return {
      windowHeight: window.innerHeight
    }
  },
  methods: {
    blur() {
      if (this.windowHeight == window.innerHeight) {
        return
      }
      window.scrollTo(0)
    }
  }
}
</script>
<style scoped>
input {
  -webkit-appearance: none;  
  outline: none
}
</style>


