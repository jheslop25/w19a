<template>
    <div>this is the song list
         <Title v-for="song in songsList" v-bind:key="song" :title="song.title" :artist="song.artist"/>
    </div>
   
</template>
<script>
import Title from './Title.vue'
export default {
    name: 'Songs',
    data : function(){
        return {
            songsList: {
                song1: {
                    title: 'a great song',
                    artist: 'john'
                },
                song2: {
                    title: 'a great song',
                    artist: 'DRAKE'
                },
                song3: {
                    title: 'a great song',
                    artist: 'DRAKE'
                }
            }
        }
    }, 
    components: {
        Title
    }
}
</script>
<style scoped>
div {
    background-color: blanchedalmond;
}
</style>