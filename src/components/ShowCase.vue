<script>
export default {
    name: 'ShowCase',
    data(){
        return{
            items : [
                {
                    src : "../assets/img/buy-comics-digital-comics.png",
                    text : 'Digital Comics'
                },
                {
                    src : "../assets/img/buy-comics-merchandise.png",
                    text : 'Dc Merchandise'
                },
                {
                    src : "../assets/img/buy-comics-subscriptions.png",
                    text : 'Subscription'
                },
                {
                    src : "../assets/img/buy-comics-shop-locator.png",
                    text : 'Comic Shop Locator'
                },
                {
                    src : "../assets/img/buy-dc-power-visa.svg",
                    text : 'Dc Power Visa'
                },
            ]
        }
    },
    methods:{
        getImagePath: function(imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="container-fluid showcase">
        <div class="container py-5">
            <div class="row row-cols-5">
            <div class="col d-flex" v-for="element in items">
                <!-- <img src="../assets/img/buy-comics-digital-comics.png" alt=""> -->
                <img :src="getImagePath(element.src)" alt=""> 
                <div class="d-flex align-items-center px-3 text-light">
                    {{element.text}}
                </div>
            </div>
        </div>
        </div>
    </div>
</template>

<!-- <style lang="scss" scoped>

</style> -->