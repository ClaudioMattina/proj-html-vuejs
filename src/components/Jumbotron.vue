<template>
  <div id="jumbo-container" class="d-flex justify-content-center align-items-center">
      <div id="content-container" class="d-flex align-items-center text-center flex-column justify-content-center">
          <div id="today-container">
              <p>TODAY'S PICK</p>
          </div>
          <h2>Food Corner: Top Japanese Restaurants for Sushi</h2>
          <p>March 25, 2019</p>
          
      </div>
  </div>
</template>

<script>
export default {
    name:"JumbotronIndex"
}
</script>

<style lang="scss" scoped>
    #jumbo-container{
        background-image: url("../assets/materiale/single-post-img3.jpg");
        background-size: cover;
        background-position: center;
        width: 100%;
        height: 700px;
        margin-top: 150px;

            #content-container{
                height: 200px;
                width: 500px;
                background-color: white;
                border-radius: 10px;
                    p{
                        margin-bottom: 50px;
                    }

                    #today-container{
                       
                       p{
                        background-color: #fc7525;
                        padding: 10px;
                        margin-bottom: 30px;
                        border-radius: 10px;
                        color: white;
                       }
                        
                    }
            }


    }
</style>