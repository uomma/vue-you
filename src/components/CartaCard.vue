
<script>
export default {
    name: 'CartaCard',
    props: {
        img: String ,
        name : String,
        type : String,


    }
}
</script>

<template>
    <div class="row col-12">
        <div class="card text-center col">
        <div class="img"><img class="img-fluid" :src="img"></div>
        <h3>{{ name }} </h3>
        <p>{{ type }}</p>


    </div>
    </div>
    
</template>


<style lang="scss" scoped></style>