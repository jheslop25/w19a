<template>
    <div>this is the song list
         <Title v-for="song in songs" v-bind:key="song" :title="song.title" :artist="song.artist"/>
    </div>
   
</template>
<script>
import Title from './Title.vue'
export default {
    name: 'Songs',
    props: {
        songs: Array
    },
    components: {
        Title
    },
    methods: {
        passSongOut: function(){
            this.$emit('addToPlayList', 'this is a song! YEAH!');
            console.log('you clicked a song!');
        }
    }
}
</script>
<style scoped>
div {
    background-color: blanchedalmond;
}
</style>