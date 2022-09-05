<template>
    <div class="container">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="Logo Digital Comics">
        </div>
            <ul class="main_list">
                <li class="list_item">
                    <a href="#">Characters</a></li>
                <li class="list_item">
                    <a href="#">Comics</a></li>
                <li class="list_item">
                    <a href="#">Movies</a></li>
                <li class="list_item">
                    <a href="#">Tv</a></li>
                <li class="list_item">
                    <a href="#">Games</a></li>
                <li class="list_item">
                    <a href="#">Collectibles</a></li>
                <li class="list_item">
                    <a href="#">Videos</a></li>
                <li class="list_item">
                    <a href="#">Fans</a></li>
                <li class="list_item">
                    <a href="#">News</a></li>
                <li class="list_item">
                    <a href="#">Shop</a></li>
            </ul>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
 
    .container {
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        padding: 1.25rem 7rem;
        margin: 0 auto;
    }

    .logo {
        width: 5rem;

    }

    .main_list {
        display: flex;
        flex-wrap: wrap;
        gap: 2rem;
        text-transform: uppercase;
        font-weight: bold;
        font-size: 0.75rem;
    }



</style>