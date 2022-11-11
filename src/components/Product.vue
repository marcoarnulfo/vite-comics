<script>
export default {
    props: {
        image: String,
        title: String,
    }
}
</script>

<template>

    <div class="col text-dark">
        <div class="card my-3">
            <img class="rounded" :src="image" alt="">
            <div class="text-center">{{ title }}</div>
        </div>
    </div>

</template>