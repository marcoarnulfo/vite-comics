<script>
export default {
    name: 'SiteHeader',
    data(){
        return{
            links : [
                {
                    text : 'Characters',
                    href : '#',
                },
                {
                    text : 'Comics',
                    href : '#',
                },
                {
                    text : 'Movies',
                    href : '#',
                },
                {
                    text : 'Tv',
                    href : '#',
                },
                {
                    text : 'Games',
                    href : '#',
                },
                {
                    text : 'Collectibles',
                    href : '#',
                },
                {
                    text : 'Videos',
                    href : '#',
                },
                {
                    text : 'Fans',
                    href : '#',
                },
                {
                    text : 'News',
                    href : '#',
                },
                {
                    text : 'Shop',
                    href : '#',
                },
            ]
        }
    }
}
</script>

<template>

    <header id="site-header">
        <div class="container d-flex justify-content-between">
            <div class="logo py-3">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>
            <div class="links d-flex align-items-center">
                <a class="p-3 fw-bolder" href="" v-for="element in links" :class="element.text == 'Comics' ? 'active' : ''">
                    {{element.text}}
                </a>
            </div>
        </div>
    </header>

</template>

<!-- <style lang="scss" scoped>

</style> -->