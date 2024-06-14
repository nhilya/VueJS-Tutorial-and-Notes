<template>
  <HelloVue/>
  <TwoWayBinding/>
  <ToggleMessage/>
  <ItemLists/>
  <ClickCounter/>
  <AreaCalculator/>
  <ChildComponent/>
  <!-- Border for VueJS Assignment -->
  <GreetingMessage/>
</template>

<script>
import HelloVue from './components/HelloVue.vue'
import TwoWayBinding from './components/TwoWayBinding.vue'
import ToggleMessage from './components/ToggleMessage.vue'
import ItemLists from './components/ItemLists.vue'
import ClickCounter from './components/ClickCounter.vue'
import AreaCalculator from './components/AreaCalculator.vue'
import ChildComponent from './components/ChildComponent.vue'
import GreetingMessage from './components/GreetingMessage.vue'


export default {
  name: 'App',
  components: {
    HelloVue,
    TwoWayBinding,
    ToggleMessage,
    ItemLists,
    ClickCounter,
    AreaCalculator,
    ChildComponent,
    GreetingMessage
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
