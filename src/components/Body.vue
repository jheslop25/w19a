<template>
    <div id="body-container">
        <Songs :songs="songs"/>
        <Playlist/>
    </div>
</template>
<script>
import Songs from './Songs.vue'
import Playlist from './PlayList'
export default {
    name: 'Body',
    components: {
        Playlist,
        Songs
    },
    data: function (){
        return {
            songs: [
                {
                    title: 'title one',
                    artist: 'artist one'
                },
                {
                    title: 'title two',
                    artist: 'artist two'
                },
                {
                    title: 'title three',
                    artist: 'artist two'
                },
                {
                    title: 'title four',
                    artist: 'artist one'
                }
            ],
            // use these lists to handle business logic
            playlist: []
        }
    }
}
</script>
<style scoped>
#body-container {
    max-width: 100vw;
    min-height: 80vh;
    background-color: bisque;
    display: grid;
    grid-template-columns: minmax(25vw, 1fr) minmax(25vw, 1fr);
    grid-template-rows: 80vh;
}
</style>