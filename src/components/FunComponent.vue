<template>
  <div>
    <button @click="change_color">Click me</button>

  </div>
</template>

<script>
export default {
 methods: {
    change_color: function (){
        document.body [`style`][`backgroundColor`] = `green`
    }
 }
 }
</script>

<style scoped>
/* add your styles here */
</style>

