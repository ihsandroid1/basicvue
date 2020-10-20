<template>
    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',

    data(){
        return {

        }
    }
}
</script>

<style>
    nav ul {
        padding: 0;
    }

    nav li{
        display: inline-block;
        list-style-type: none;
        margin-right: 10px;
        text-decoration: none;
        color: green;
    }

    nav li a {
        text-decoration: none;
    }

    nav {
        text-align: center;
    }

</style>