<template>
    <div>
        <p>{{ title }}</p>
        <p>{{ artist }}</p>
        <button  @click="clickedSong(title, artist)">Add to Play List</button>
    </div>
</template>
<script>
export default {
    name: 'Title',
    props: {
        title: String,
        artist: String,
        
    },
    methods: {
        clickedSong: function(title, artist){
            console.log('you clicked ' + title + ' by ' + artist);
            this.$emit('addSong', title, artist);
        }
    }
}
</script>
<style scoped>

</style>