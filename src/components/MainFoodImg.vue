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
    
</style>