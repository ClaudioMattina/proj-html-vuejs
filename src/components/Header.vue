<template>
  <div class="my-container d-flex">

    <div class="top-container d-flex justify-content-between">

        <div id="download" class="d-flex ">
          <p>Download App</p>
          <div id="ios-container">
              <a class="d-flex" href="#">iOS</a>
          </div>
          <p>Advertise whit us</p>
        </div>

        <div class="d-flex social">
            <p>F</p>
            <p>INS</p>
            <p>TWI</p>
            <p>YT</p>
        </div>

    </div>
      
  </div>
</template>

<script>
export default {
    name: "HeaderIndex"
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