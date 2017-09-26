<template>
  <div class="all">
    <menutop></menutop>
    <start></start>
  </div>
</template>

<script>
  import menutop from '@/components/menutop'
  import start from '@/components/start'

  export default {
    components: {
      menutop,
      start
    },
    data() {
      return {
      }
    }
  }
</script>

<style lang="scss">
  // @import './assets/css/main.scss';
  .all {
    // background: #EBECF3;
  }
</style>
