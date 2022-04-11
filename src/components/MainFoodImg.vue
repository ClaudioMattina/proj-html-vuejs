<template>
  <div>
      <div class="row mt-5">
          <!-- lista immagini -->
          <div class="col-8 p-0 d-flex flex-wrap">
              <div v-for="(element,index) in imgList" :key="index" class="my-card">
                  <div class="img-container">
                      <img :src="element.url" alt="">
                  </div>
                  <div class="d-flex align-items-center flex-column mt-3 text-center px-3">
                      <h5> {{ element.text }} </h5>
                      <p> {{ element.paragraph }} </p>
                  </div>
              </div>
              <div id="more-post" class="d-flex justify-content-center align-items-center">
                  <a href="#">LOAD MORE POSTS</a>
              </div>
          </div>

          <!-- social e commenti -->
          <div class="col-4 mt-3">
              <input id="search-bar" placeholder="Search..." type="text">
              <p>Follow Us</p>
              <div class="social-icons d-flex align-items-center">
                  <span><i class="fa-brands fa-facebook-f"></i></span>
                  <span><i class="fa-brands fa-instagram"></i></span>
                  <span><i class="fa-brands fa-twitter"></i></span>
                  <span><i class="fa-brands fa-youtube"></i></span>
                  <span><i class="fa-brands fa-pinterest-p"></i></span>
              </div>

              <div class="popular-recent d-flex my-5">
                  <div id="popular" class="active">
                      <a href="#">POPULAR</a>
                  </div>
                  <div id="recent">
                      <a href="#">RECENT</a>
                  </div>
              </div>

              <div v-for="(element,index) in socialComment" :key="index" class="info d-flex align-items-center">
                  <div class="info-img me-3">
                      <img :src="element.url" alt="">
                  </div>
                  <div class="info-content">
                      <h3>{{element.text}}</h3>
                      <p> {{element.date}} </p>
                  </div>
              </div>

               <!-- tweets -->
             <div id="tweets" class="col-4 mt-5">

                <div class="d-flex justify-content-between">
                    <div id="tweets-title d-flex">
                        <p><span class="fs-3">Tweets</span> by <a href="#"> @Teme_Fusion </a></p>
                    </div>
                    <div class="d-flex justify-content-center align-items-center">
                        <a class="mb-2" href="#"> <img src="../assets/materiale/image.svg" alt="icona delle info"> </a>
                    </div>
                </div>

                <!-- sottoscheda tweet -->
               <div class="row">
                   <div class="col-1 d-flex p-0">
                       <img id="my-logo" src="../assets/materiale/3a74ce3d0532b7773b174c45ca3bd05a_normal.png" alt="">
                   </div>
                   <div class="col-11">
                       <div id="icon-tw-container" class="d-flex justify-content-between align-items-center">
                           <h5>TemeFusion</h5>
                           <img src="../assets/materiale/image (1).svg" alt="">
                       </div>
                       <div id="tweet-content">
                           <p>@Theme_fusion</p>
                           <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Blanditiis explicabo quis minima dolore placeat atque laudantium veritatis ratione! Molestiae, nisi consequuntur exercitationem quas ipsam iure vero sapiente ab nihil maxime.</p>
                       </div>
                        <!-- blocco img dello sconto -->
                        <div id="img-sconto">
                            <img src="../assets/materiale/En2TRxLW4AEiWUN.jpeg" alt="">
                        </div>
                        <div id="condividi-like" class="d-flex justify-content-between">
                            <div id="ciao" class="d-flex align-items-center mt-2">
                                <img class="me-2" src="../assets/materiale/image (2).svg" alt="">
                                <img src="../assets/materiale/image (3).svg" alt="">
                            </div>
                            <div class="mt-2"><p>21h</p></div>
                        </div>
                   </div>
               </div> 
             </div> 
          </div>

         
          
      </div>
  </div>
</template>

<script>

export default {
    name:"MainFoodImgIndex",

    data:function(){
        return{
            imgList:[
                {
                    url:require("../assets/materiale/fi-roundup.jpg"),
                    text:"Roundup: My New Favourite Recipes for Healthy Living",
                    paragraph:"By admin | March 25th, 2019"
                },
                 {
                    url:require("../assets/materiale/fi-korean-food.jpg"),
                    text:"Mcal Prep: Korean Bibimpap with kimchi",
                    paragraph:"By admin | March 25th, 2019"
                },
                 {
                    url:require("../assets/materiale/fi-toasts.jpg"),
                    text:"Why these Toasts with Tea are My Favourite",
                    paragraph:"By admin | March 25th, 2019"
                },
                 {
                    url:require("../assets/materiale/fi-street-food.jpg"),
                    text:"Exploring Street Food in Bangkock",
                    paragraph:"By admin | March 25th, 2019"
                },
                 {
                    url:require("../assets/materiale/fi-organic-breakfast.jpg"),
                    text:"Organic Choices for Healthier Living",
                    paragraph:"By admin | March 25th, 2019"
                },
                 {
                    url:require("../assets/materiale/fi-water-side-rest.jpg"),
                    text:"5 Waterside Restaurants in Instambul for Special Events",
                    paragraph:"By admin | March 25th, 2019"
                },
            ],
            socialComment:[
                {
                    url:require("../assets/materiale/single-post-img3.jpg"),
                    text:"Food Corner: Top Japanese Restaurants for Sushi",
                    date:"March 25th, 2019"
                },
                {
                    url:require("../assets/materiale/singapore-featured-image.jpg"),
                    text:"City Guide: Singapore",
                    date:"March 25th, 2019"
                },
                {
                    url:require("../assets/materiale/slide1-bg-66x66.jpg"),
                    text:"6 Nutritionals Tips to Help Burn Body Fat",
                    date:"March 25th, 2019"
                },
            ]
            /* aggiungere condizione active ai bottoni */
        }
    }
}
</script>

<style lang="scss" scoped>

    .col-8{
        gap: 40px;
        #more-post{
            background-color: #f0eeeb;
            width: 100%;
            height: 50px;
            a{
                font-size: 1rem;
                text-decoration: none;
                color: black;
            }
        }
    } 
    .my-card{
        width: calc((100% / 2) - 30px );
        height: 350px;
        background-color: white;
        .img-container{
            width: 100%;
            height: 65%;
            img{
                width: 100%;
                height: 100%;
            }
        }
        h3{
            font-size: 1.4rem;
        }
        p{
            font-size: 0.8rem;
        }
    }
    #more-post{
        margin-bottom: 150px;
    }
    .col-4{
        #search-bar{
            width: 100%;
            border-radius: 3px;
            padding: 3px;
            border: 1px solid #f0eeeb;
            margin-bottom: 30px;
        }
        p{
            color: #fc7525;
        }
        .social-icons{
            font-size: 1.5rem;
            span{
                background-color: #f0eeeb;
                border: 1px solid #f0eeeb;
                 border-radius: 5px;
                 margin: 0px 10px;
                 width: 30px;
                 height: 30px;
                 display: flex;
                 justify-content: center;
                 align-items: center;
            }
            i{
                font-size: 1rem;
                color: #6a6b6c;
            }
        }
        .popular-recent{
            width: 100%;
            height: 50px;
            a{
                color: black;
                text-decoration: none;
            }
           #popular{
               width: 50%;
               height: 100%;
               border: 1px solid #f0eeeb;
               display: flex;
               justify-content: center;
               align-items: center;
           }
           #recent{
                width: 50%;
                height: 100%;
                border: 2px solid #f0eeeb;
                display: flex;
                justify-content: center;
                align-items: center;
           }
           .active{
               background-color: white;
           }
        }
        .info{
            width: 100%;
            height: 100px;
            .info-img{
                width: 60px;
                height: 60px;
                img{
                    width: 100%;
                    height: 100%;
                    border-radius: 100%;
                }
            }
            .info-content{
                h3{
                    font-size: 0.8rem;
                }
                p{
                    font-size: 0.6rem;
                    color: #6a6b6c;
                }
            }
        }
    }
    #tweets{
        background-color: white;
        padding: 30px;
        border-radius: 10px;
        width: 100%;

        #my-logo{
            height: 40px;
        }
        p{
            color: black;
            font-size: 0.8rem;
            }
        #tweets-title{
            width: 100%;          
        }
    }
    #icon-tw-container{
        height: 20px;
        width: 100%;
        margin-top: 10px;
        margin-left: 5px;
        h5{
            font-size: 1rem;
            font-weight: bold;          
        }
        img{
            height: 100%;  
        }
    }
    #img-sconto{
        width: 100%;
        margin-top: 30px;
        img{
            width: 100%;
            border-radius: 5x;
        }
    }

    #condividi-like{
            height: 20px;
            #ciao{
                height: 100%;
                img{
                    height: 100%;
                }
            }
            
        }
    
</style>