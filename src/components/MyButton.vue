<template >
    <div>
        <h1 v-on:mousemove="getMove()">My Mouse Move</h1>
        <!-- <button v-on:click="getData('button 1 press kiya')">Click Me</button>
        <button v-on:dblclick="getData('button 2 is clicked')">Click Me</button> -->
        <button v-on:click="getData()">Incerment</button>
        <button v-on:click="getData1()">Derement</button>
        <h2>{{ count }}</h2>
    </div>
</template>
<script>
export default {
    name: "MyButton",
    data() {
        return {
            count: 0
        }
    },
    methods: {

        getData() {

            this.count = this.count + 1;

        },
        getData1() {

            this.count = this.count - 1;

        },
        getMove() {
            console.warn("function called")
        }
    }
}
</script>
<style scoped>
button {
    padding: 10px
}
</style>