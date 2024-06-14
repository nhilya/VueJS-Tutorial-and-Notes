<template>
  <h1>Assignment Question 2</h1>
  <h2>Two Way Binding</h2>
  <div>
    <input v-model="message" placeholder="Type something" />
    <p>You typed: {{ message }}</p>
  </div>
</template>

<script>
export default {
  name: 'TwoWayBinding',
  data() {
    return {
      message: ''
    }
  }
}
</script>

<style scoped>
h1 {
    color: #42b983;
}
</style>