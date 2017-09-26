<template>
  <div>
    <header>
        <div class="header margin container justify-content-center align-items-start">
          <div class="block-header">
            <div class="logo container column justify-content-center align-items-center">
              <img src="../assets/images/top.svg" width="100" class="logo1">
              <img src="../assets/images/logo.svg" width="300">
            </div>
            <div class="text">
              <h1>Create your SEO and study</h1>
            </div>
            <div class="button">
              <nuxt-link to="/start" class="start">Start now</nuxt-link>
            </div>
          </div>
        </div>
    </header>
  </div>
</template>

<script>
  export default {
    name: 'topo',
    data() {
      return {


      }
    }
  }
</script>

<style lang="scss" scoped>
.header {
  min-height: 100vh;
  background: #3a5eec;
  // background: linear-gradient(90deg, #5f72bd, #3a5eec)
  background: url(../assets/images/bg.svg), linear-gradient(140deg, #3f62ec 50%, #3a5eec 50%);
  background-size: 100%;
  background-repeat: repeat-x;
  background-attachment: fixed;
  background-position: bottom;
    .block-header {
      padding-top: 15vh;
      width: 600px;
      max-width: 90%;
      color: #fff;
      text-align: center;
      .text {
        padding-top: 20px;
        h1  {
          font-size: 1rem;
        }
      }
      .button {
        .start {
          height: 40px;
          line-height: 60px;
          background: #fff;
          padding: 10px 40px 10px 40px;
          border-radius: 4px;
          color: #3A5EEC;
          font-size: 14px;
          font-weight: 700;
          transition: .1s;
          text-transform: uppercase;
          &:hover {
            background: #FFDD67;
            color: #EBA352
          }
        }

      }
      .logo {
        .logo1 {
          padding-bottom: 20px;
          animation-name: top;
          animation-duration: 1s;
          animation-iteration-count: infinite;
          animation-timing-function: linear;
          animation-fill-mode: backwards;
          @keyframes top {
            0% {
            }
            50% {
              transform: scale(1.5, 1.5) rotate(10deg);
            }
            100% {
            }
          }
        }
      }
    }
}
</style>
