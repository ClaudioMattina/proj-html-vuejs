<template>
  <div>
      <!-- TOP PARAGRAFO E BOTTONE -->
      <div id="top-content" class="row">
          <div class="col-12 d-flex align-items-center justify-content-between p-0">
              <div id="paragrph-container">
                   <h3>FARM TO TABLE</h3>
                   <p>Aliquam eat volupat. Ut quis ligula a magna blamdit firibus. Suspendisse maximus lacus non nunc lacinia lobortis.</p>
              </div>
              <div>
                  <a href="#">READ OUR BLOG <span><i class="fa-brands fa-jenkins"></i></span></a>
              </div>
          </div>
      </div>

      <!-- IMMAGINE GRANDE E ROBA -->
      <div class="row mt-5">
          <!-- scheda -->
          <div id="container-main-scheda" class="col-8 shadow p-0">
              <div id="big-img-container">
                  <img src="../assets/materiale/single-post-img3.jpg" alt="">
              </div>
              <div id="paragrafo-big-img" class="p-4">
                  <h5 class="mt-3">Food Corner: Top Japanese Restaurant for Sushi</h5>
                  <p id="admin-p">by Admin | March 25th, 2019</p>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta, aut laboriosam eum atque cum consequuntur molestias accusantium earum alias, illum harum perspiciatis quia corporis doloremque consectetur nam dolore maxime dolor?</p>
                  <div class="d-flex justify-content-between">
                      <p> Read more <span> <a href="#"> <i class="fa-solid fa-chevron-right"> </i> </a> </span> </p>
                      <span><i class="fa-regular fa-comments"></i> 0 </span>
                  </div>
              </div>
          </div>

          <!-- al lato della scheda -->
          <div class="col-4">
            <!-- immagine con commento centrato -->
            <div id="img-for-comment" class="d-flex text-center justify-content-center align-items-center">
                <div id="comment-container" class="justify-content-center d-flex">
                    <h3>VIEW OUR LATEST RECIPES</h3>
                </div>
            </div>
            <!-- immagine scheda -->
            <div id="giuda-scheda" class="mt-5">
                <div id="img-guida" class="">
                    <p>City Guide: Singapore</p>
                </div>
                <div id="all-guide" class="d-flex justify-content-center align-items-center">
                    <a href="#"> <span class=" me-1"><i class="fa-solid fa-earth-americas"></i></span> VIEW ALL CITY GUIDES</a>
                </div>
            </div>

            <div id="bar" class="mb-2"></div>
          </div>
      </div>

      
  </div>
</template>

<script>
export default {
    name:"MainContentIndex"
}
</script>

<style lang="scss" scoped>
    #top-content{
        margin-top: 150px;
        #paragrph-container{
        width: 50%;
        }
        a{
            text-decoration: none;
            color: white;
            background-color: #fc7525;
            font-size: 1rem;
            padding: 10px 20px;
        }
    }
    #container-main-scheda{
        background-color: white;
            #paragrafo-big-img{
                #admin-p{
                    font-size: 0.8rem;
                    border-bottom: 1px dotted #afafaf;
                    padding-bottom: 20px;
                }
            }

            #big-img-container{
                width: 100%;
                height: 500px;
                img{
                width: 100%;
                height: 100%;
                }
            }
    }
    #img-for-comment{
        background-image: url("../assets/materiale/ad-bg.jpg");
        background-position: center;
        background-size: cover;
        width: 100%;
        height: 450px;
           #comment-container{
               width: 50%;              
                 h3{
                     font-size: 1.3rem;      
                 }
           }
    }
    #giuda-scheda{
        width: 100%;
        height: 300px;
        #img-guida{
        width: 100%;
        height: 200px;
        background-image: url("../assets/materiale/singapore-featured-image.jpg");
        background-position: center;
        background-size: cover;
        position: relative;
            p{
                background-color: black;
                color: white;
                position: absolute;
                top: 130px;
                padding: 5px;
            }
        }
        #all-guide{
            width: 100%;
            height: 40px;
            background-color: #fc7525;
            a{
                color: white;
                font-size: 0.8rem;
                text-decoration: none;                
            }
        }
    }
    #bar{
        border-bottom: 2px solid lightgray;
    }
    
    

</style>