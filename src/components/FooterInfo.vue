<template>
  <div id="my-container" class="mt-5">
      <div class="row">
          <div id="logo-icons-contsainer" class="col-3 d-flex flex-column">
              <div id="img-logo">
                  <img src="../assets/materiale/avada-food-logo.png" alt="">
              </div>
              <div id="icone-social" class="d-flex gap-3">
                <p><i class="fa-brands fa-facebook-f"></i></p>
                <p><i class="fa-brands fa-instagram"></i></p>
                <p><i class="fa-brands fa-twitter"></i></p>
                <p><i class="fa-brands fa-youtube"></i></p>
              </div>
          </div>

          <div id="info-list" class="col-3 d-flex justify-content-start">
              <ul>
                  <li v-for="(element,index) in info" :key="index"><a href="#"> {{element}} </a></li>
              </ul>
          </div>
          
          <div id="info-contatti" class="col-3 d-flex flex-column">
              <h2 class="title">CONTACT</h2>
              <div class="row">
                  <div class="col-2">
                      <i class="fa-solid fa-location-dot"></i>
                  </div>
                  <div class="col-10">
                      <p>775 New York Ave</p>
                      <p>Brooklyn Kings, New York 11203</p>
                  </div>
                  <div class="col-2">
                      <i class="fa-solid fa-phone"></i>
                  </div>
                  <div class="col-10">
                      <p>+0100-505-0000</p>
                  </div>
                  <div class="col-2">
                      <i class="fa-solid fa-envelope"></i>
                  </div>
                  <div class="col-10">
                      <p>info@your-domain.com</p>
                  </div>
              </div>
          </div>
          <div class="col-3">
              <h2 class="title mb-5">GET OUR APP</h2>
              <div class="app-img">
                  <img src="../assets/materiale/download-android.png" alt="">
              </div>
              <div class="app-img">
                  <img src="../assets/materiale/download-app-store.png" alt="">
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"FooterInfoIndex",
    data:function(){
        return{
            info:["Recipes", "Places", "Blog", "About", "Contact"]
        }
    }
}
</script>

<style lang="scss" scoped>
    #my-container{
        width: 70%;
        margin: 0 auto;
        
    }
    .col-3{
        padding: 10px;
    }

    #logo-icons-contsainer{
    }

    #img-logo{
        width: 70%;
        
        img{
            width: 100%;
        }
    }
    #icone-social{
        color: grey;
        margin-top: 25px;
        margin-left: 5px;
    }
    #info-list{
        border-left: 1px grey dotted;
        border-right: 1px grey dotted;
        ul{
            list-style: none;
            li{
                padding: 10px 0px;
                a{
                    text-decoration: none;
                    color: black;
                }
            }
        }
    }
    .title{
        color: #fc7525;
        font-size: 1.2rem;
    }
    #info-contatti{
        color: grey;
        border-right: 1px grey dotted;
    }
    .app-img{
        height: 30%;
        img{
            height: 60%;
        }
    }

</style>