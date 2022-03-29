<template>

  
    <div class="Header-container">
    <div id="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>

    <div id="nav-list">
      <ul>

       <li v-for="(link,index) in headerLinks" :key="index">
           <a :class="{active : link.current}" href="#"> {{link.text}} </a>
        </li>

      </ul>
    </div>
  </div>
  
  

</template>

<script>

export default {
  name: "HeaderComponentIndex",
  data: function(){
    return{
      headerLinks:[
        {
          text: "CHARACTERS",
          url: "#",
          current: false,
        },
        {
          text: "COMICS",
          url: "#",
          current: false,
        },
        {
          text: "MOVIE",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "GAMES",
          url: "#",
          current: false,
        },
        {
          text: "COLLECTIVES",
          url: "#",
          current: false,
        },
        {
          text: "VIDEOS",
          url: "#",
          current: false,
        },
        {
          text: "FANS",
          url: "#",
          current: false,
        },
        {
          text: "NEWS",
          url: "#",
          current: false,
        },
        {
          text: "SHOP",
          url: "#",
          current: false,
        },
      ]
    }
  }
};

</script>

<style lang="scss" scoped>

    .Header-container{
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 70%;
      margin: 0 auto;

         ul{
           display: flex;
           
            li{
              list-style-type: none;
              padding: 10px;
              
              
              
                a{
                  text-decoration: none;
                  color: black;
                  font-size: 1rem;
                  
                    &:active,
                    &.active{
                      color: rgb(4, 84, 189);
                      border-bottom: 2px solid rgb(4, 84, 189);
                    }
                }

            }
         }
    }
</style>
