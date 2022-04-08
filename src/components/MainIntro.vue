<template>
  <div id="main-intro-wrapper" class="shadow">
     <div class="row p-4">
         <div class="col-12 d-flex justify-content-center align-items-center mb-3">
             <div class="my-border"></div>
             <h4>FOODDIE JOURNAL</h4>
             <div class="my-border"></div>
         </div> 

         <div v-for="(element,index) in foodsJurnal" :key="index" class="my-card col-4 d-flex flex-column">

            <div class="img-container">
               <img src="../assets/materiale/single-post-img3.jpg" alt="">
            </div>
            <div class="d-flex flex-column align-items-center text-center content-container">
               <h5 class="my-3"> {{element.text}} </h5>
               <p> {{element.paragraph}} </p>
            </div>

         </div>

     </div>
  </div>
</template>

<script>
export default {
    name:"MainIntroIndex",

    data:function(){
        return{
            foodsJurnal:[
                {
                    url:"../assets/materiale/single-post-img3.jpg",
                    text:"Food Corner: Top Japanese Restaurant Sushi",
                    paragraph:"By Admin, 1 March 25th, 2019"
                },
                {
                    url:"../assets/materiale/fi-roundup.jpg",
                    text:"Rounddup: My New Favourite Recipes For Healthy Living",
                    paragraph:"By Admin, 1 March 25th, 2019"
                },
                {
                    url:"../assets/materiale/fi-toasts.jpg",
                    text:"Why These Toasts whit Tea are My New Favourite",
                    paragraph:"By Admin, 1 March 25th, 2019"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #main-intro-wrapper{

        width: 70%;
        background-color: white;
        position: absolute;
        left: 50%;
        top: 550px;
        transform: translate(-50%);
        margin-bottom: 200px;
        
        

            h4{
                margin: 0px 20px;
            }
            .my-border{
                border-bottom: 1px dotted #afafaf;
                width: 30%;
            }

            .my-card{
                
               h5{
                   font-size: 1rem;
               }
                p{
                    font-size: 0.6rem;
                }
                .img-container{
                    width: 100%;
                    height: 150px;
                    img{
                        width: 100%;
                        height: 100%;
                    }
                }
            }
    }
</style>