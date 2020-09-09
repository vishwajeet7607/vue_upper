<template>
<div>
    <h1> App Convert String To Upper Case</h1>
    <form @submit="upper">
        <input v-model="message" placeholder="give me a  string">
        <h1>output </h1>
        <p> {{ message|capitalize }}</p>
    </form>
</div>
</template>

<script>
export default {
    name: 'AddUpper',
    data() {
        return {
            message: [""],

        }
    },
    methods: {
        upper() {
            // message = this.message.toUpperCase

            // return message.toUpperCase()

        }
    },
    filters: {
        capitalize: function (value) {
            if (!value) return ''
            value = [value]
            value = value.toString()
            value
            return value.toUpperCase()
        }
    }

    //     //
}
// props: {
//     message: String
// },

// filters: {
//     capitalize: function (value) {
//         if (!value) return ''
//         value = [value]
//         value = value.toString()
//         value
//         return value.toUpperCase()

//     //         // return value.charAt(0).toUpperCase() + value.slice(1)

// // 
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
}
</style>
