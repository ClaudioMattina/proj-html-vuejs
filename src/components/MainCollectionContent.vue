<template>
  <div
  >
      <div id="title" class="row my-5">
        <div class="col-12 d-flex flex-column">
            <h3>CULINARY COLLECTION</h3>
            <p>Aliquam eat volupat. Ut quis ligula a magna blamdit firibus. Suspendisse maximus lacus non nunc lacinia lobortis.</p>
        </div>
      </div>

      <div class="row">

        <div v-for="(element, index) in imagesList" :key="index" class="col-3 my-wrapper">
          <div class="img-container">
            <img :src="element.url" alt="">
          </div>
          <div class="description d-flex justify-content-center align-items-center">
            <h5> {{ element.text }} </h5>
          </div>
        </div>

      </div>

  </div>
</template>

<script>
export default {
    name:"MainCollectionContent",

    data:function(){
      return{
        imagesList: [
          {
            url: require("../assets/materiale/drinks-recipes.png"),
            text:"DRINKS"
          },
          {
            url:require("../assets/materiale/soups-recipes.png"),
            text:"SOUPS"
          },
          {
            url:require("../assets/materiale/baking-recipes.png"),
            text:"BAKERY"
          },
          {
            url:require("../assets/materiale/dinner-recipes.png"),
            text:"DINNER"
          },
          {
            url:require("../assets/materiale/healthy-recipes.png"),
            text:"HEALTHY"
          },
          {
            url:require("../assets/materiale/staff-picks.png"),
            text:"STAFF PICKS"
          },
          {
            url:require("../assets/materiale/premium-recipes.png"),
            text:"APPETISERS"
          },
          {
            url:require("../assets/materiale/quick-easy-recipes.png"),
            text:"QUICK & EASY"
          },
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
    #title{
      width: 70%;
      margin: 0 auto;
      text-align: center;
    }

    .img-container{
      height: 150px;
      width: 100%;
      background-color: white;

        img{
          width: 100%;
          height: 100%;
        }
    }

    .description{
      margin-bottom: 20px;
      background-color: white;
      h5{
        font-size: 1rem;
       
      }
    }

</style>