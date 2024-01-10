<script>
import CartaCard from './CartaCard.vue';
import axios from 'axios';
export default {
    name: 'CardList',
    components: {
        CartaCard
    },
    data() {
        return {
            cards: [],
        }
    },
    created() {
        axios.get(' https://db.ygoprodeck.com/api/v7/cardinfo.php')
        .then((response)=>{
            console.log(response);
            this.cards= response.data.data;
        })

    }
}
</script>

<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-12 col-sm-5 " v-for="(card, index) in cards.slice(0,20)">
<!-- per visualizzare le img dato che con card.card_images.image_url ti dice che img: undefined DEVI METTER LA POSIZIONE INDEX!!!  -->
                <CartaCard :img="card.card_images[0].image_url" :name="card.name"  :type="card.type"/>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped></style>