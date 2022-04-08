<template>

  <div class="my-container">
      

    <div class="top-container d-flex justify-content-between">

        <div id="download" class="d-flex ">
          <p>Download App</p>
          <div id="ios-container">
              <a class="d-flex" href="#">iOS</a>
          </div>
          <p>Advertise whit us</p>
        </div>

        <div class="d-flex social">
            <p><i class="fa-brands fa-facebook-f"></i></p>
            <p><i class="fa-brands fa-instagram"></i></p>
            <p><i class="fa-brands fa-twitter"></i></p>
            <p><i class="fa-brands fa-youtube"></i></p>
        </div>

    </div>

    <div class="row my-3">
        <div class="col-12 d-flex justify-content-center align-items-center">
            <img src="../assets/materiale/avada-food-logo.png" alt="">
        </div>
    </div>
      <HeaderList />
  </div>
</template>

<script>
import HeaderList from './HeaderList.vue'

export default {
    name: "HeaderIndex",
    components: {
        HeaderList
    }
}
</script>

<style lang="scss" scoped>


    .my-container{
        width: 70%;
        margin: 0 auto;
        height: 100px;
        margin-top: 20px;

        .top-container{
            width: 100%;

            .social{
                p{
                    margin: 0px 5px;
                }
            }

            #download{
             height: 20px;

            #ios-container{
                margin: 0px 15px 0px 10px;
                border: 1px solid #fc7525;
                background-color: #fc7525;
                border-radius: 5px;
                
                a{
                    text-decoration: none;
                    color: white;
                    padding: 0px 10px 2px 10px;

                }
            }
            }
        }
         
         
    }
</style>