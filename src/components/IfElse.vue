<template>
    <div>
        <!-- <h1 v-if="show"> If Condition</h1>
        <h1 v-else> Else Condition</h1>

        <br>
        <br>
        <button v-on:click="show = !show">Toggle</button>

        <hr> -->
        <br>

        <input type="text" maxlength="2" v-model="checkPersonAge"
            oninput="this.value = this.value.replace(/[^0-9.]/g, '').replace(/(\..*?)\..*/g, '$1');">
            <h1 v-if="checkPersonAge>=18">Your Are Eligible to drive</h1>
            <h1 v-else>Your Are not Eligible to drive</h1>
        <p>{{ checkPersonAge }}</p>
        <br>
        <br>
        <br>

    </div>
</template>

<script>
export default {
    name: "IfElse",
    data() {
        return {
            show: true,
            member: '',
            checkPersonAge: '18'
        }
    }
}
</script>

<style scoped>

</style>
