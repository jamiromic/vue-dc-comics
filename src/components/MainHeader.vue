<template>
    <div class="container">
        <div class="logo">
            <img src="../assets/dc-logo.png" alt="Logo Digital Comics">
        </div>
            <ul class="main_list">
               <li v-for="(item,i) in dataHeader" :key="i" class='list_item'> {{ item }} </li>
            </ul>
    </div>
</template>

<script>
    import dataHeader from '../dataHeader'

    export default {
    components: {  
    },
    data() {
        return {
            dataHeader: dataHeader
        }
    }
}
</script>

<style lang="scss" scoped>
 
    .container {
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        margin: 0 auto;
        max-width: 1600px;
        height: 100px;
    }

    .logo {
        width: 4rem;

    }

    .main_list {
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        gap: 2rem;
        text-transform: uppercase;
        font-weight: bold;
        font-size: 0.75rem;
        height: 100%;
    }

    .list_item {

        display: flex;
        align-items: center;
        height: 100%;
        cursor: pointer;

        &:hover {
            color:  #0282F9;
            border-bottom: 5px solid #0282F9;
            padding-top: 5px;
        }

    }


</style>