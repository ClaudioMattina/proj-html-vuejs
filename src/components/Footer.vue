<template>
  <div id="my-footer">
    <FooterSubscribe/>
    <FooterImg/>
    <FooterInfo/>
    <FooterCopyright/>
  </div>
</template>

<script>
import FooterSubscribe from './FooterSubscribe.vue'
import FooterImg from './FooterImg.vue'
import FooterInfo from './FooterInfo.vue'
import FooterCopyright from './FooterCopyright.vue'
export default {
    name: "FooterIndex",
    components:{
      FooterSubscribe,
      FooterImg,
      FooterInfo,
      FooterCopyright
    }
}
</script>

<style lang="scss" scoped>
  #my-footer{

  }
</style>