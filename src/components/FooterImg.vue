<template>
  <div id="Imgs-container" class="d-flex">
      <div v-for="(element,index) in imgsList" :key="index" class="my-img">
          <img :src="element.url" alt="">
      </div>
  </div>
</template>

<script>
export default {
    name:"FooterImgIndex",
    data:function(){
        return{
            imgsList:[
                {
                    url:require("../assets/materiale/Yogurt-Nan.jpg")
                },
                {
                    url:require("../assets/materiale/Mixed-fruits.jpg")
                },
                {
                    url:require("../assets/materiale/r-rachel-park-366508-unsplash-min.jpg")
                },
                {
                    url:require("../assets/materiale/r-michelle-tsang-500721-unsplash-min.jpg")
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #Imgs-container{
        width: 100%;
        .my-img{
            width: calc(100% / 4);
            img{
                width: 100%;
            }
        }
    }
</style>