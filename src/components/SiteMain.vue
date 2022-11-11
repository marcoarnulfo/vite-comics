<script>
import ShowCase from './ShowCase.vue';
import Jumbotron from './Jumbotron.vue'
// import dcComics from '../data/dc-comics';
import Product from './Products.vue';
export default {
    name: 'SiteMain',
    components: {
        ShowCase,
        Jumbotron,
        //dcComics,
        Product,
    },
    // data() {
    //     return {
    //         dcComics
    //     }
    // }
}
</script>

<template>

    <main id="site-main">
        <Jumbotron />
        <Product/>
        <!-- <div class="container-fluid bg-dark">
            <div class="container p-3">
                <div class="row">
                    <div v-for="film in dcComics" class="col text-dark">
                        <div class="card">
                            <img class="rounded" :src="film.thumb" alt="">
                            <div class="text-center">{{ film.series }}</div>
                        </div>
                    </div>
                </div>
            </div>
        </div> -->
        <ShowCase />
    </main>

</template>

<!-- <style lang="scss" scoped>

</style> -->