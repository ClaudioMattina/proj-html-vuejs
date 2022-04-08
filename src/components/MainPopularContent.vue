<template>
  <div>
      <div class="row my-3">
          <div  id="my-introduction" class="col-8 d-flex justify-content-center align-items-center flex-column text-center">
              <h3>POPULAR RECIPES</h3>
              <p>Aliquam eat volupat. Ut quis ligula a magna blamdit firibus. Suspendisse maximus lacus non nunc lacinia lobortis.</p>
          </div>
      </div>

      <div class="row">

        <div id="big-card" class="col-6">

            <div id="img-container">
                <img src="../assets/materiale/Yogurt-Nan.jpg" alt="">
            </div>

            <div id="content-card" class="p-3">
                <h5>Lunch Favourite with Salad, Naan and Beans</h5>
                <p id="sub-title">Bakery, Featured, Healthy, Lates Recipes, Staff Picks.</p>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Sunt ipsam, laboriosam blanditiis fugiat odio nemo veniam alias explicabo. Possimus fugiat adipisci eos! Velit, veniam inventore omnis ex provident odio impedit.</p>
                <a href="#">LEARN MORE</a>
            </div>
        </div>

        <div class="col-6">
            <div class="img-list-containers">
                <img src="../assets/materiale/Mixed-fruits.jpg" alt="">
            </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"MainPopularContentIndex",

    data:function(){
        return{
            images:[
                {
                    url:"../assets/materiale/Mixed-fruits.jpg"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #my-introduction{
        margin: 0 auto;
        margin-top: 100px;
    }

    #big-card{
        height: 500px;
        width: 40%;
        background-color: white;
        padding: 0;

        #img-container{
            height: 50%;
            width: 100%;

            img{
                width: 100%;
                height: 100%;
            }
        }

        #content-card{
            
            h5{
                font-size: 1.2rem;
            }
            #sub-title{
                font-size: 0.7rem;
                border-bottom: 1px dotted #afafaf;
                padding-bottom: 15px;
            }

            p{
                font-size: 1rem;
            }

            a{
                text-decoration: none;
                color: white;
                background-color: #fc7525;
                padding: 10px;
                font-size: 0.8rem;
            }
        }
    }

    .img-list-containers{
        
    }
   

</style>