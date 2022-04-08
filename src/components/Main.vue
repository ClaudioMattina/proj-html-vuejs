<template>
  <div id="my-main">

    <div class="my-container">

      
      
      <MainPopularContent />

      <MainCollectionContent />

    </div>

  </div>
</template>



<script>


import MainPopularContent from './MainPopularContent.vue'
import MainCollectionContent from './MainCollectionContent.vue'

export default {
    name: "MainIndex",
    components:{
      MainPopularContent,
      MainCollectionContent
    }
}
</script>

<style lang="scss" scoped>
    #my-main{
      background-color: #f6f7f1;
    }

    .my-container{
      width: 70%;
      margin: 0 auto;
    }
</style>