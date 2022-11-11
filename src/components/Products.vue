<script>
import dcComics from '../data/dc-comics';
import Product from './Product.vue'

export default {
    name : 'Products',
    components: {
        dcComics,
        Product
    },
    data() {
        return {
            dcComics
        }
    }
}
</script>


<template>
    <div class="container-fluid bg-dark">
            <div class="container p-3">
                <div class="row">
                    <div class="serie">
                    <span class="text-light fw-bolder series rounded">CURRENT SERIES</span>
                </div>
                    <Product v-for="film in dcComics" :image="film.thumb" :title="film.series" />
                    <!-- <div v-for="film in dcComics" class="col text-dark">
                        <div class="card">
                            <img class="rounded" :src="film.thumb" alt="">
                            <div class="text-center">{{ film.series }}</div>
                        </div>
                    </div> -->
                </div>
                <div class="text-center py-5">
                    <span class="text-light fw-bolder load rounded">LOAD MORE</span>
                </div>
                
            </div>
        </div>
</template>


<style lang="scss" scoped>
.serie{
    margin-top: -2.5rem;
}

</style>