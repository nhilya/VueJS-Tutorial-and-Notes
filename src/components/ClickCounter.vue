<template>
    <div id="app">
        <h1>Assignment Question 5</h1>
        <h2>Hello Vue Component</h2>
        <h2>Counter: {{ counter }}</h2>
        <button @click="increment">Increase number</button>
        <br><br>
        <button @click="decrement">Decrease number</button>
        <br><br>
        <button @click="reset">Reset number to 0</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            counter: 0
        }
    },
    watch: {
        counter(newValue, oldValue) {
            console.log('Counter changed from', oldValue, 'to', newValue)
        }
    },
    methods: {
        increment() {
            this.counter++
        },
        decrement() {
            this.counter--
        },
        reset() {
            this.counter = 0
        }
    }
}
</script>

<style scoped>
h1 {
    color: #42b983;
}
</style>