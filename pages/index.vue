<template>
  <div>
  <topo></topo>
  <app></app>
  <rodape></rodape>
  </div>
</template>

<script>
  import topo from '@/components/topo';
  import app from '@/components/app';
  import rodape from '@/components/footer';

  export default {
    components: {
      topo, app, rodape
    },
    data() {
      return {
      }
    }
  }
</script>

<style lang="scss">
  @import './assets/css/main.scss';
</style>
