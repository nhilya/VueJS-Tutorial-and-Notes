<template>
    <h1>Assignment Question 3</h1>
    <h2>Conditional Rendering</h2>
    <div>
        <button @click="toggleMessage">{{ messageVisible ? 'Hide' : 'Show' }} Message</button>
        <p v-if="messageVisible">You have clicked the toggle, now you can see the message!</p>
    </div>
</template>

<script>
export default {
    name: 'ToggleMessage',
    data() {
        return {
            messageVisible: false
        }
    },
    methods: {
        toggleMessage() {
            this.messageVisible = !this.messageVisible
        }
    }
}
</script>

<style scoped>
h1 {
    color: #42b983;
}
</style>