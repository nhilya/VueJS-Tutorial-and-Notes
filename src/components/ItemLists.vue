<template>
    <h1>Assignment Question 4</h1>
    <h2>List Rendering</h2>
    <div>
        <ul>
            <li v-for="(item, index) in items" :key="index">{{ item }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'ItemList',
    data() {
        return {
            items: ['Item 1', 'Item 2', 'Item 3', 'Item 4', 'Item 5']
        }
    }
}
</script>

<style scoped>
h1 {
    color: #42b983;
}
</style>