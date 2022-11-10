<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteMain from './components/SiteMain.vue';
import SiteFooter from './components/SiteFooter.vue';

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter,
  }
}
</script>

<template>

  <SiteHeader />
  <!-- /#site-header -->

  <SiteMain />
  <!-- /#site-main -->


  <SiteFooter />
  <!-- /#site_footer -->

</template>

<!-- <style lang="scss" scoped>

</style> -->
