<template>
    <div id="playlist">this is the playlist
       <Title v-for="song in songs" v-bind:key="song" :title="song.title" :artist="song.artist"/>
    </div>
</template>
<script>
import Title from './Title'
export default {
    name: 'Playlist',
    props: {
        songs: Array
    },
    components: {
        Title
    }
}
</script>
<style scoped>
#playlist {
    
    height: 70vh;
    background-color: blanchedalmond;
}
</style>