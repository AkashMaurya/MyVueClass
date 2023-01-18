<template >
    <div>
        <!-- <h2>this is home {{ email }}</h2> -->
        <!-- <h2>Mobile {{ mobile }}</h2> -->
        <!-- directly value assign kiya aur ye overRide ho gya sabhi mobile me its not possible in anguler-->
        <h2>Mobile {{ mobile=9000 }}</h2>

        <!-- its checking the value its correct or not ,the output will be given in boolean true and false-->
        <h2>Mobile {{ mobile== 9000 }}</h2>
        <!-- <h2>Function {{ getName("prakash") }} Coder</h2> -->
        <h2>MyEmail {{ getData().email }}</h2>
    </div>
</template>
<script>
export default {
    name: "HomeView",
    data(){
        return{
            email:'akash@abc.com',
        }
    },
    methods:{
        getData(){    
            return{
                email:this.email
            }
        }
    }
}


</script>
<style scoped>
h2 {
    color: purple;
    background-color: aqua;
}
</style>