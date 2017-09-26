<template>
  <div class="menu">
    <div class="menu-space size margin container justify-content-between align-items-center">
      <div class="logo">
        <img src="../assets/images/logo.svg" width="100">
      </div>
      <div class="links">
        <nuxt-link to="/">Home</nuxt-link>
        <nuxt-link to="/start">Start</nuxt-link>
      </div>
    </div>
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
.menu {
  width: 100%;

  background: linear-gradient(140deg, #3f62ec 50%, #3a5eec 50%);
    .menu-space {
      height: 70px;
        .links {
          a {
            color: #fff;
            margin-right: 10px;
            opacity: .7;
            transition: .1s;
              &:hover {
                opacity: 1
              }
          }
        }
    }
}
</style>
