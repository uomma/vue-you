<script>
import CarteSearch from './CarteSearch.vue';
import CardList from './CardList.vue';
    export default {
        name:'AppMain',

        components: {
            CarteSearch,
            CardList,
        }
    }
</script>

<template>
<main>
    <CarteSearch></CarteSearch>
    <CardList></CardList>
</main>
</template>



<style lang="scss" scoped>

</style>