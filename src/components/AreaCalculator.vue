<template>
    <h1>Assignment Question 6</h1>
    <h2>Computed Properties</h2>
    <div>
        <label for="length">Length: </label>
        <input id="length" v-model.number="length" type="number" placeholder="Enter length" />
        <br><br>
        <label for="width">Width: </label>
        <input id="width" v-model.number="width" type="number" placeholder="Enter width" />

        <p>Calculated Area: {{ area }}</p>
    </div>
</template>

<script>
export default {
    name: 'AreaCalculator',
    data() {
        return {
            length: 0,
            width: 0
        }
    },
    computed: {
        area() {
            return this.length * this.width
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