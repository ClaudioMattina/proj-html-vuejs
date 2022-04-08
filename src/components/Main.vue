<template>
  <div id="my-main">

    <div class="my-container">

       
      
      <MainPopularContent />

      <MainCollectionContent />

      <MainContent />

    </div>

  </div>
</template>



<script>


import MainPopularContent from './MainPopularContent.vue'
import MainCollectionContent from './MainCollectionContent.vue'
import MainContent from './MainContent.vue'

export default {
    name: "MainIndex",
    components:{
      MainPopularContent,
      MainCollectionContent,
      MainContent
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