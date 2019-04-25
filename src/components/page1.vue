<template>
  <div>
    <h1>这是page1</h1>

  </div>
</template>

<script>


  export default {
    components: {},
    data(){
      return {
        isLoading: true
      }
    },
    created(){
      this.getData()
    },
    mounted(){

    },
    methods: {
      getData(){

      }
    },

  }
</script>

<style lang="scss" scoped>
  //@import "/bocm/platformjs/static/css/common.css";
</style>
