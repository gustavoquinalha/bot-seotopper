<template>
  <div class="size margin">
    <div class="title-intro container justify-content-center align-items-center">
      <h1>Just type the data and generate the meta tags for your website</h1>
      <div class="mark">
      </div>
    </div>
    <div class="item">
      <div class="title">
        <h1>General information about your website</h1>
        <div class="mark">
        </div>
      </div>

      <form class="" v-model="seo">
        <div class="container wrap">

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">Page title</label>
            <input type="text" name="" v-model="seo.title" placeholder="Type a title">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">Page description</label>
            <input type="text" name="" v-model="seo.description" placeholder="Type a description">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">Author</label>
            <input type="text" name="" v-model="seo.author" placeholder="Type a author">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">image</label>
            <input type="text" name="" v-model="seo.image" placeholder="Type a image">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">canonical</label>
            <input type="text" name="" v-model="seo.canonical" placeholder="Type a canonical">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">robots</label>
            <input type="text" name="" v-model="seo.robots" placeholder="Type a robots">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">base</label>
            <input type="text" name="" v-model="seo.base" placeholder="Type a base">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">siteMap</label>
            <input type="text" name="" v-model="seo.siteMap" placeholder="Type a siteMap">
          </div>

          <div class="box-form flex-basis-400 flex-grow-1 container column">
            <label for="">themeColor</label>
            <input type="text" name="" v-model="seo.themeColor" placeholder="Type a themeColor">
          </div>


        </div>

      </form>
    </div>

    <div class="btn-esp container align-items-center ">
      <button type="button" class="btn" name="button">GENERATE</button>
    </div>

  </div>
</template>

<script>
export default {
  name: 'app',
  data() {
    return {
      seo: {
        title: 'titulo',
        description: 'descricao',
        author: 'autor',
        image: 'imagem',
        canonical: 'canonical',
        robots: 'robots',
        base: 'bbase',
        siteMap: 'sitemap',
        themeColor: 'themecolor',
      }
    }
  }
}
</script>

<style lang="scss" scoped>
.btn-esp {
  margin-bottom: 50px;
}
// background: linear-gradient(90deg, #5f72bd, #3a5eec)
.item {
    background: #fff;
    box-shadow: 0 0 20px 0 rgba(0,0,0,.1);
    box-sizing: border-box;
    padding: 30px;
    margin-top: 50px;
    margin-bottom: 25px;
    border-radius: 4px;
}
.title {
  padding-bottom: 40px;
  h1 {
    font-size: 1.5rem;
    // opacity: .7;
    color: #3a5eec
  }
  .mark {
    width: 100px;
    height: 10px;
    background: #FCDE6D;
    border-radius: 4px
  }
}
.box-form {
  padding: 10px;
  padding-bottom: 20px;
  box-sizing: border-box;
  label {
    font-weight: 700;
    opacity: .7;
    font-size: 16px;
    margin-bottom: 5px;
  }
  input {
    height: 40px;
    font-size: 14px;
    line-height: 40px;
    padding-left: 10px;
    box-sizing: border-box;
    border-radius: 4px;
    border: none;
    // background: #f7f7f7;
    border: 1px solid #ddd;
    color: #808080
  }
}
.title-intro {
  padding-top: 50px;
  width: 500px;
  margin: 0 auto;
  text-align: center;
  h1 {
    font-size: 1.5rem;
    // color: #3a5eec;
    opacity: .7

  }
}
</style>
