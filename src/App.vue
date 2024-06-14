<template>
  <GreetingMessage/>
  <!-- Border for VueJS Assignment -->
  <HelloVue/>
  <TwoWayBinding/>
  <ToggleMessage/>
  <ItemLists/>
  <ClickCounter/>
  <AreaCalculator/>
  <ChildComponent/>
  <!-- Border for VueJS Assignment -->
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

