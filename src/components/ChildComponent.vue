<template>
    <h1>Assignment Question 7 & 8</h1>
    <h2>Computed Properties</h2>
    <div>
      <p>Message from parent: {{ message }}</p>
      <button @click="emitEvent">Click me</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ChildComponent',
    props: {
      message: {
        type: String,
        required: true
      }
    },
    methods: {
      emitEvent() {
        this.$emit('childClicked', 'Child component button was clicked!')
      }
    }
  }
  </script>
  
  <style scoped>
  h1 {
      color: #42b983;
  }
  p {
      color: #c45924;
  }
  </style>
  