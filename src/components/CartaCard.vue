
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
    <div class="card text-center">
        <div class="img"><img class="img-fluid" :src="img"></div>
        <h3>{{ name }} </h3>
        <p>{{ type }}</p>


    </div>
</template>


<style lang="scss" scoped></style>