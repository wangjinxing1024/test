<template>
  <div>
    <h1 @click="$router.push('/page2')">这是page1</h1>

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

<style scoped>

</style>
