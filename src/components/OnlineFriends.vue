<template>
    <div id="online-friends">
        <h2>Online Friends</h2>
         <div v-for="teman in friends" :key="teman">
            <span v-if="teman.online"> {{ teman.name }} </span>
        </div>
    </div>
</template>

<script>
export default {
    name : 'OnlineFriends',
    props : ['friends'],
    data(){
           return{
            
        }
    }
}
</script>

<style>
</style>