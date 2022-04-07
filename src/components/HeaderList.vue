<template>
  <div>
      <ul class="d-flex justify-content-around">
          <li v-for="(element,index) in navBarList" :key="index">
              <a :class="{active : element.current}" href="#"> {{ element.text }} </a>
          </li>
      </ul>
      
  </div>
</template>

<script>
export default {
    name: "HeaderListIndex",

    data: function(){
        return{
            navBarList:[
                {
                    text: "Home",
                    current: true,
                },
                {
                    text: "Recipes",
                    current: false,
                },
                {
                    text: "Places",
                    current: false,
                },
                {
                    text: "Blog",
                    current: false,
                },
                {
                    text: "About",
                    current: false,
                },
                {
                    text: "Contact",
                    current: false,
                },
                {
                    text: "icona",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

    li{
        list-style: none;
        margin: 10px;
    }
    a{
        text-decoration: none;
        color: black;

            &:active,
            &.active,
            &:hover{
                color: #fc7525;
                border-bottom: 2px solid #fc7525;
            }
    }
</style>