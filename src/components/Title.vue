<template>
    <div>
        <p>{{ title }}</p>
        <p>{{ artist }}</p>
    </div>
</template>
<script>
export default {
    name: 'Title',
    props: {
        title: String,
        artist: String
    }
}
</script>
<style scoped>

</style>