<template>
    <div id="all-friends">
        <h2>All Friends</h2>
        <div v-for="teman in friends" :key="teman">
            <span @click="unfriend(teman.name)"> {{ teman.name }} </span>
        </div>
    </div>
</template>

<script>
export default {
    name : 'Allfriends',
    props : ['friends'],
    data(){
        return{
          
        }
    },
    methods : {
        unfriend(name){
            this.$emit('delete', { name })
        }
    }
}
</script>

<style>
</style>