<script>
import ShowCase from './ShowCase.vue';
export default {
    name: 'SiteMain',
    components:{
        ShowCase
    }
}
</script>

<template>

    <main id="site-main">
        <div class="container-fluid bg-dark d-flex">
            <div class="container py-5">
                <h1 class="text-light fw-bolder"> Content goes here </h1>
            </div>
        </div>
        <ShowCase/>
    </main>

</template>

<!-- <style lang="scss" scoped>

</style> -->