<template>
    <div>
        <h1 @click="$router.push('/')">这是page2</h1>
    </div>
</template>

<script>
  //import loading from '@/components/'

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

<style>

</style>
