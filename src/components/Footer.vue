<template>
  <div id="my-footer">
    <FooterSubscribe/>
    <FooterImg/>
  </div>
</template>

<script>
import FooterSubscribe from './FooterSubscribe.vue'
import FooterImg from './FooterImg.vue'
export default {
    name: "FooterIndex",
    components:{
      FooterSubscribe,
      FooterImg,
    }
}
</script>

<style lang="scss" scoped>
  #my-footer{

  }
</style>