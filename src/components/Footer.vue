<template>
  <div id="my-footer">
    <FooterSubscribe/>
  </div>
</template>

<script>
import FooterSubscribe from './FooterSubscribe.vue'
export default {
    name: "FooterIndex",
    components:{
      FooterSubscribe,
    }
}
</script>

<style lang="scss" scoped>
  #my-footer{
    
  }
</style>