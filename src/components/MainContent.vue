<template>
    <div class="container">
        <div class="hero">
            <button>CURRENT SERIES</button>
        </div>
        <div class="wrapper">
            <ComicCard v-for="(card,i) in dataCard" :key="i" :src="card.thumb" :titolo="card.series" />
        </div>
        <button>LOAD MORE</button>
        

    </div>
</template>

<script>
    import dataCard from '../dataCard'
    import ComicCard from './ComicCard.vue'


    export default {
        components: {
            ComicCard
        },
        data() {
            return {
                dataCard: dataCard
            }
        }
        
    }
</script>

<style lang="scss" scoped>

    .container {
        background-color: #1C1C1C;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-bottom: 1.75rem;
        

        .wrapper {

            color: white;
            max-width: 1500px;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 1rem;
            padding: 3.5rem 1.5rem 0.5rem;
            margin: 0 auto;
            
        }

        button {
            width: fit-content;
            background-color:  #0282F9;
            color: white;
            padding: 0.75rem 4rem;
            font-weight: 700;
            border: none;

        }

        .hero {
            background-image: url(../assets/jumbotron.jpg);
            background-size: cover;
            height: 350px;
            width: 100vw;
            position: relative;

            button {
                font-size: 1.25rem;
                padding: 0.75rem 1.25rem;
                position: absolute;
                bottom: -22px;
                left: 200px;
            }
        }
    }

</style>