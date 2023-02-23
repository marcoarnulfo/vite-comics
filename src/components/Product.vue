<script>
export default {
    props: {
        image: String,
        title: String,
    }
}
</script>

<template>

    <div class="col text-white">
        <div class="card bg-dark my-3">
            <img class="rounded" :src="image" alt="">
            <div class="text-center">{{ title }}</div>
        </div>
    </div>

</template>

<style scoped>
img{
    width: 300px;
    height: 400px;
}
</style>