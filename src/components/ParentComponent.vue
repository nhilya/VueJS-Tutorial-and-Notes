<template>
    <div>
      <h2>Parent Component</h2>
      <ChildComponent :message="parentMessage" @childClicked="handleChildClick" />
    </div>
  </template>
  
  <script>
  import ChildComponent from './ChildComponent.vue'
  
  export default {
    name: 'ParentComponent',
    components: {
      ChildComponent
    },
    data() {
      return {
        parentMessage: 'Hello from Parent!'
      }
    },
    methods: {
      handleChildClick(message) {
        alert(message);
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
  