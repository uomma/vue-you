<script>
import { store } from '../store';
export default {
    name: 'Search',
    data(){
        return{
            store,

        }
    },
    methods:{
        test(){
            console.log('modulo inviato')
            
        }
    }
}
</script>

<template>
    <div class="container">
        <form @submit.prevent="$emit('search')">
            <div class="row justify-content-center">
                <div class="mb-3 col-12 col-sm-auto">
                    <label for="search-card" class="form-label d-none">Search</label>
                    <input type="text" class="form-control" id="search-card" aria-describedby="emailHelp"
                        placeholder="search card" v-model="store.searchKey">
                </div>
                <div class="mb-3col-12 col-sm-auto">
                    
                    <select class="form-select" id="search-card" v-model="store.selectCard">
                        <option selected value="">select card</option>
                        <option>One</option>
                        <option>Two</option>
                        <option>Three</option>
                    </select>
                </div>
                <div class="mb-3col-12 col-sm-auto">
                    <button type="submit" class="btn btn-primary">Search</button>

                </div>

            </div>
        </form>
    </div>
</template>



<style lang="scss" scoped></style>