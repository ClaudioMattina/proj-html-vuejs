<template>
  <div id="my-footer">
    <FooterSubscribe/>
    <FooterImg/>
    <FooterInfo/>
  </div>
</template>

<script>
import FooterSubscribe from './FooterSubscribe.vue'
import FooterImg from './FooterImg.vue'
import FooterInfo from './FooterInfo.vue'
export default {
    name: "FooterIndex",
    components:{
      FooterSubscribe,
      FooterImg,
      FooterInfo
    }
}
</script>

<style lang="scss" scoped>
  #my-footer{

  }
</style>