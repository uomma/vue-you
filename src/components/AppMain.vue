<script>
import CarteSearch from './CarteSearch.vue';
import CardList from './CardList.vue';
    export default {
        name:'AppMain',

        components: {
            CarteSearch,
            CardList,
        },
        methods:{
            handleSearch(){
                console.log('ho ascoltato')
                this.$emit('algo')
            }
        }

    }
</script>

<template>
<main>
    <CarteSearch @search="handleSearch" ></CarteSearch>
    <CardList></CardList>
</main>
</template>



<style lang="scss" scoped>

</style>