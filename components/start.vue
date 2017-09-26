<template>
  <div class="start">
    <div class="size margin">

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
.start {
  background: #EBECF3;
  height: calc(100vh - 70px);
}
.resposta {
  background: #ddd;
  position: fixed;
  bottom: 0;
  width: 100%;
  border-top: 1px solid rgba(0,0,0,.1)
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
      transition: .1s;
      box-shadow: 0 0 10px 0 rgba(0,0,0,.5);
        svg {
          transform: translateX(-1px);
          transition: .1s;
        }
        &:hover {
          background: #FFDD67;
            svg {
              stroke: #3A5EEC;
              fill: #FFDD67
            }
        }
    }
}
</style>
