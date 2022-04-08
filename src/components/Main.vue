<template>
  <div id="my-main">

    <div class="my-container">

      <MainIntro />
      
      <MainPopularContent />

    </div>

  </div>
</template>



<script>
import MainIntro from './MainIntro.vue'
import MainPopularContent from './MainPopularContent.vue'

export default {
    name: "MainIndex",
    components:{
      MainIntro,
      MainPopularContent
    }
}
</script>

<style lang="scss" scoped>
    #my-main{
      /* background-color: #f6f7f1; */
      background-color: aquamarine;
    }

    .my-container{
      width: 70%;
      margin: 0 auto;
    }
</style>