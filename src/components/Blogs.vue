<template>
    <div class="blogs">
        <h2>Blogs Ihsan</h2>
        <div v-for="post in posts" :key="post.id">
            <h3>{{post.title}}</h3>
            <p>{{ post.body }}</p>
        </div>
    </div>
</template>

<script>

import axios from 'axios'

export default {

    name : 'Blogs',
    data() {
        return {
           posts : [] 
        }
    },
    methods: {
  
    },
    
    created(){
        axios.get('https://jsonplaceholder.typicode.com/posts/')
        .then(res => {
            console.log(res)
            this.posts = res.data
        })
    }

}
</script>

<style>
    button {
        padding: 10px 25px;
        border-radius: 50px;
        outline: none;
        background-color:goldenrod;
        color:honeydew;
        border: none;
        cursor: pointer;
    }

    .blogs{
        width: 800px;
        margin: auto;
        text-align: left;
        box-shadow: 0px 0px 30px 15px #B9B5B4
    }

    h2,h3,p{
        margin-left: 20px;
    }

  
</style>