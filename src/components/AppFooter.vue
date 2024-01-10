<script>

import { store } from '../store';
    export default {
        name:'AppFooter',
        data(){
            return{
                store
            }
        }
    }
</script>

<template>
   <footer class="text-center my-5">
    risultati trovati : {{store.cardsFound }}
   </footer>
</template>



<style lang="scss" scoped>

</style>