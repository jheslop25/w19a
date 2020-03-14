<template>
    <div><h4>{{ title }}</h4></div>
</template>
<script>
export default {
    name: 'Header',
    props: {
        title: String
    }
}
</script>
<style scoped>
div {
    width: 100vw;
    height: 10vh;
    background-color: aqua;
}
</style>