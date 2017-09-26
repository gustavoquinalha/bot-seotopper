<template>
  <div class="">
    <!-- <nuxt-link to="/">Home</nuxt-link>
    <nuxt-link to="/start">Start</nuxt-link> -->
  </div>
</template>

<script>
export default {
  name: 'topo',
  data() {
    return {
      showMenu: false
    }
  },
  methods: {
    toggleShowMenu() {
      this.showMenu = !this.showMenu
    }
  }
}
</script>

<style lang="scss" scoped>
</style>
