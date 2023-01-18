<template >
    <div>
        <h1 v-if="show"> If Condition</h1>
        <h1 v-else> Else Condition</h1>
      
        <br>
        <br>
        <button v-on:click="show=!show">Toggle</button>
    </div>
</template>
<script>
export default {
    name: "IfElse",
    data() {
        return {
            show: true
        }
    }

}
</script>
<style scoped>

</style>