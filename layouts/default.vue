
<template>
  <div id="app">
      <!-- <menutop></menutop> -->
    <keep-alive>
      <nuxt/>
    </keep-alive>

  </div>
</template>

<script>
  import menutop from '@/components/menutop';

  export default {
    name: 'app',
    components: {
      menutop
    },
    mounted() {},
    data() {
      return {}
    }
  }
</script>

<style lang="scss">
  @import './assets/css/main.scss'
</style>
