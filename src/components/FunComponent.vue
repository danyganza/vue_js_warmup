<template>
  <div>
    <button @click="change_color">Click me</button>
     <section>
      <p v-for="(secret, i) in secrets" :key="i" @click="make_text_pink">
        {{ secret }}
      </p>
    </section>

  </div>
</template>

<script>
export default {

  data() {
    return {
      secrets: [
        `Did you know that ball is life?`,
        `Did you know that drinking water is good for your overall health`,
      ],
    };
  },

 methods: {
    change_color: function (){
        document.body [`style`][`backgroundColor`] = `green`
    },
    make_text_pink(details) {
      details[`target`][`style`][`color`] = `pink`;
    },
 }
 }
</script>

<style scoped>
</style>

