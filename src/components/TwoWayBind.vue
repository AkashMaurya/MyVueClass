<template>
    <div>
        <!-- <input type="text" placeholder="Type the Text Here" id=input spellcheck="true" v-model="count">
        <h1>{{ count }}</h1> -->
        <input type="text" placeholder="Enter the Email" class="input" v-model="email"><br><br>
        <input type="password" placeholder="Enter the Password" class="input" v-model="password"><br><br>
        <p>Your Hobbies</p>
        <label for="Singing">Singing</label>
        <input type="checkbox" value="Singing" v-model="hobbies" id="Singing">

        <label for="Dancing">Dancing</label>
        <input type="checkbox" value="Dancing" v-model="hobbies" id="Dancing">

        <label for="Writing">Writing</label>
        <input type="checkbox" value="Writing" v-model="hobbies" id="Writing">
        <br><br>


        <p>Gender</p>
        
        <input type="radio" id="male" value="Male" v-model="who">
        <label for="male">Male</label>

        <input type="radio"  id="female" value="Female" v-model="who">
        <label for="female">Female</label>
        
        <br><br>

        <br>
        
        <h2>Selected Hobbies: {{ hobbies }}</h2>
        <h2>Selected gender : {{ who }}</h2>
        <br><br><br>
        <button v-on:click="getData()">Get Values</button>
        <br><br><br><br><br><br><br>
    </div>

</template>

<script>
export default {
    name: "TwoWayBindComponent",
    data() {
        return {
            email: null,
            password: null,
            hobbies: [],
            who: null,

        }
    }
}
//     methods: {
//         getData() {
//       }      // this.count=document.getElementById("input").value
//             console.warn(`Your Email is ${this.email} and password is ${this.password} ,'\n' Your Hobbies are ${this.hobbies} and your gender is ${this.gender}`)
//         }
//     }
// }
</script>

<style scoped>
.input {
    padding: 10px;

}

.input:focus {
    border: 1px solid red;
    background: rgb(0, 255, 21);
}
</style>
