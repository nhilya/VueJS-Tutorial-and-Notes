<template>
    <div class="greeting">
      <h1>{{ greetingMessage }}</h1>
    </div>
  </template>
  
  <script>
  export default {
    name: 'GreetingMessage',
    data() {
      return {
        currentHour: new Date().getHours()
      };
    },
    computed: {
      greetingMessage() {
        if (this.currentHour < 12) {
          return "Good Morning! Hope you're well today!";
        } else if (this.currentHour < 18) {
          return 'Good Afternoon! Make sure you have a good lunch ya!';
        } else {
          return "Good Evening! It's time to relax and have some fun!";
        }
      }
    }
  };
  </script>
  
  <style scoped>
  .greeting {
    text-align: center;
    margin-top: 50px;
    font-family: Arial, sans-serif;
  }
  
  h1 {
    font-size: 2em;
    color: #42b983;
  }
  </style>
  