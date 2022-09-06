<template>
    <div class="card">
        <div class="picture">
            <img :src="src" :alt="titolo">
       </div>
        <h4>{{ titolo }}</h4>
    </div>
</template>

<script>
    export default {
        props: {
            src: String,
            titolo: String,
        }
        
    }
</script>

<style lang="scss" scoped>

    .card {

        gap: 1rem;
        width: 195px;
        padding-bottom: 2rem;
        

        

        .picture{

            width: 180px;
            height: 180px;
            overflow: hidden;
            
        }

        h4 {
            color: rgba(255, 255, 255, 0.829);
            text-transform: uppercase;
            font-size: 0.74rem;
            font-weight: 200;
            padding-top: 1rem;
        }

        
    }

</style>