<template>
  <div id="bg-image" class="d-flex justify-content-center align-items-center flex-column">
      <!-- container titolo -->
     <div id="my-container" class="py-5 justify-content-center align-items-center">
          <h1 class="mb-4">Subscrive <span id="my-span">&</span> Recive a Free eBook</h1>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Minima eaque, minus, a, sequi earum reprehenderit corrupti nostrum eligendi culpa delectus at cum fuga libero quod?</p>

        <!-- container input -->
        <div id="input-container" class="d-flex justify-content-center">
            <div id="text-input">
                <input id="ciao" placeholder="Insert your email..." type="text">
            </div>
            <div id="button">
                <a href="#">SUBSCRIBE</a>
            </div> 
        </div>
        <p class="mt-5">Cras porttitos pellentesque sem eu pretium.</p>
     </div>
    
    
  </div>
</template>

<script>
export default {
    name:"FooterSubscribeIndex"
}
</script>

<style lang="scss" scoped>
    #bg-image{
        background-image: url("../assets/materiale/subscribe-sec-bg.png");
        background-position: center;
        background-size: cover;
        width: 100%;
        #my-container{        
            width: 70%;
            margin: 0 auto;
            text-align: center;
             #my-span{
            color: #fc7525;
            }

            #input-container{
            width: 90%;
            text-align: center;
            margin-top: 40px;
            
                #text-input{
                    width: 60%;
                    #ciao{
                        width: 80%;
                    }
                }             
            }
        }
        #button{
            width: 30%;
            a{
                text-decoration: none;
                color: white;
                background-color: #fc7525;
                padding: 10px 15px;
            }
        }  



    }
</style>