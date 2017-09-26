<template>
<div class="start">
  <div class="content-talk">
    <div class="size margin space-talk">

      <div class="talk container justify-content-start align-items-start">
        <div class="box-photo">
          <div class="photo container justify-content-center align-items-center">
              <img src="../assets/images/top.svg" width="30">
          </div>
        </div>
        <div class="mensagem flex-grow-1">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor
          in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </div>
      </div>

      <div class="talk container justify-content-start align-items-start">
        <div class="mensagem flex-grow-1">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        </div>
        <div class="box-photo">
          <div class="photo right">
          </div>
        </div>
      </div>

    </div>
  </div>
  <div class="resposta">
    <div class="size margin container size-resposta align-items-center justify-content-center">
      <div class="input-block container align-items-center justify-content-center">
        <input type="text" name="" value="" class="input" placeholder="Digite aqui sua resposta">
        <div class="esp-send container justify-content-end">
          <div class="send">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="#3A5EEC" stroke="#FFDD67" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-navigation"><polygon points="3 11 22 2 13 21 11 13 3 11"></polygon></svg>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'start',
  data() {
    return {

    }
  },
  methods: {

  }
}
</script>

<style lang="scss" scoped>
.talk {
    margin-bottom: 50px;
    .box-photo {
        width: 60px;
        max-width: 60px;
        min-width: 60px;
        .photo {
            width: 40px;
            height: 40px;
            background: #3A5EEC;
            border-radius: 50%;
            &.right {
                float: right;
            }
        }
    }
    .mensagem {
        padding: 20px;
        box-sizing: border-box;
        border-radius: 4px;
        box-shadow: 0 0 10px 0 rgba(0,0,0,.1);
        background: #fff;
        font-size: 14px;
        opacity: 0.6;
        line-height: 20px;
    }
}
.content-talk {
    // background: red;
    height: calc(100vh - 160px);
    overflow: scroll;
    padding: 50px;
    box-sizing: border-box;
}

.start {
    // background: #EBECF3;
    height: calc(100vh - 70px);
}
.resposta {
    background: #ddd;
    position: fixed;
    bottom: 0;
    width: 100%;
    border-top: 1px solid rgba(0,0,0,.1);
}
.size-resposta {
    height: 100px;
}
.input-block {
    width: 100%;
    .input {
        width: 100%;
        border: none;
        border-radius: 20px;
        height: 40px;
        box-sizing: border-box;
        padding-left: 20px;
        box-shadow: 0 0 10px 0 rgba(0,0,0,.2);
        font-size: 14px;
    }
    .esp-send {
        width: 50px;
    }
    .send {
        background: #3A5EEC;
        width: 40px;
        height: 40px;
        border-radius: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        transition: 0.1s;
        box-shadow: 0 0 10px 0 rgba(0,0,0,.5);
        svg {
            transform: translateX(-1px);
            transition: 0.1s;
        }
        &:hover {
            background: #FFDD67;
            svg {
                stroke: #3A5EEC;
                fill: #FFDD67;
            }
        }
    }
}
</style>
