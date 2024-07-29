<template>

<!-- <h1> Name : {{ getName("SAURABH KUMAR") }}</h1>

<h2>Name : {{ getName ("Raju kumar ")}}</h2>

<h1> Name2 : {{ getData().email }}</h1>

<h1>Name3 : {{getData().name }}</h1> -->

<button  v-on:click="getData()"> Click Me</button> 
<br>
<br>
<button  v-on:dblclick="getData('Button double clicked')"> Click Me</button>

<h2>{{ count }}</h2>

</template>

<script>
export default {
    name: 'HomePage',
   
    data(){
        return {
            count:0
        }
    },


    methods:{
        getData(data)
        {
            this.count=10
        }
    },

    // methods: {
    //     getName(name) {
    //         return name
    //     },
    //     getData() {
    //         return {
    //             name: "saurabh",
    //             email: this.email
    //         }
    //     }

    // }

}
</script>

<style scoped>
h1 {
    color: blue
}
</style>

<style scoped>
h2{
    color: brown;
}
</style>
