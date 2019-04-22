<template>
  <div class="hello">
    <div>{{msg}}</div>
    <!-- <img src="./score_bg.png" alt="" style="width:100%;" id="pic"> -->
    <!-- <vue-q-art :config="config" :downloadButton="downloadButton"></vue-q-art> -->

    <!-- <div style="width:400px;height:400px">
      <vue-qr :logoSrc="src2" :text="text" :dotScale = '.9' height="300" width="300"></vue-qr>
    </div> -->

  </div>
</template>

<script>
// import VueQArt from 'vue-qart'
import VueQr from 'vue-qr'


export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      /*config: {
          value: 'https://www.baidu.com',
          imagePath: '',
          filter: 'color',
          size: 500
      },
        downloadButton: false*/
        // text:'https://www.baidu.com',
        // src2:'./static/logo.png',
        items: ['1', '2', '3', '5', '6', '7', '8', '9', '10'],
        end: 10,
        refreshing: false
    }
    
  },
  mounte(){

  },
  methods:{
    back () {
      window.history.back()
    },
    refresh () {
      this.refreshing = true
      setTimeout(() => {
        this.refreshing = false
        var arr = []
        for (let i = this.end; i < this.end + 10; i++) {
          arr.push(String(i + 1))
        }
        this.end += 10
        this.items = arr
      }, 2000)
    }},

  components: {VueQr}


}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  height:400px;
}

</style>
