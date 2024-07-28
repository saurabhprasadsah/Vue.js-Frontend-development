<template>
<h1> Email : {{ email }}</h1>

<h1> Name : {{ getName("SAURABH KUMAR") }}</h1>
<h1> Name2 : {{ getData().email }}</h1>
</template>

<script>
export default {
    name: 'HomePage',
    data() {
        return {
            email: 'kumarsaurabh2910@gmail.com',
        }
    },

    methods: {
        getName(name) {
            return name
        },
        getData() {
            return {
                name: "saurabh",
                email: this.email
            }
        }

    }

}
</script>

<style scoped>
h1 {
    color: blue
}
</style>
