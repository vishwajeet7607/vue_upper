<template>
<div id="app">
    <Header />
    <AddUpper />

</div>
</template>

<script>
import AddUpper from './components/AddUpper';
import Header from './components/Header';
export default {
    name: 'App',

    components: {
        Header,
        AddUpper
    },

}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2a5077;
    margin-top: 0px;
    height: 20px;
}
</style>
