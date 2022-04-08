<template>
  <div>
      <!-- TOP PARAGRAFO E BOTTONE -->
      <div id="top-content" class="row mt-5">
          <div class="col-12 d-flex align-items-center justify-content-between">
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
      <div class="row">
          <div class="col-8">
              <div id="big-img-container">
                  <img src="" alt="">
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
    

</style>