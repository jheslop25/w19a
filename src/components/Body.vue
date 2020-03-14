<template>
    <div id="body-container">
        <Songs/>
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