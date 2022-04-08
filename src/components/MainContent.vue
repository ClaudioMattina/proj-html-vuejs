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
          <div class="col-4"></div>
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
    
    

</style>