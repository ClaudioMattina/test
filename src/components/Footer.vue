<template>

  <div id="my-container">
      <div id="lists-footer-container">

          <div id="links-footer">

              <div class="link">

                <h4>DC COMICS</h4>
                <ul>
                    <li v-for="(link,index) in comicsLinks" :key="index"><a href="#"> {{link.text}} </a></li>
                </ul>  
              </div>

              <div class="link">
                <h4>DC</h4>
                <ul>
                    <li v-for="(link,index) in dcLinks" :key="index"><a href="#"> {{link.text}} </a></li>
                </ul>
              </div>
              
              <div class="link">
                <h4>SITES</h4>
                <ul>
                    <li v-for="(link,index) in sitesLinks" :key="index"><a href="#"> {{link.text}} </a></li>
                </ul>
              </div>

              <div class="link">
                <h4>SHOP</h4>
                <ul>
                    <li v-for="(link,index) in shopLinks" :key="index"><a href="#"> {{link.text}} </a></li>
                </ul>
              </div>

          </div>
          <div id="bg-container">
                <div id="img-footer">
                </div>
          </div>
          
      </div>

      <div id="grey-container"> 
          <div id="social-footer-container">

          <div>
                <div id="my-btn">
                    <a href="#">SIGN-UP NOW!</a>
                </div>          
          </div>

          <div id="icons-social-container">
              <h3>FOLLOW US</h3>
              <div class="social-icon">
                  <img src="../assets/img/footer-facebook.png" alt="">
              </div>
              <div class="social-icon">
                  <img src="../assets/img/footer-periscope.png" alt="">
              </div>
              <div class="social-icon">
                  <img src="../assets/img/footer-pinterest.png" alt="">
              </div>
              <div class="social-icon">
                  <img src="../assets/img/footer-twitter.png" alt="">
              </div>
              <div class="social-icon">
                  <img src="../assets/img/footer-youtube.png" alt="">
              </div>
          </div>
        </div>
      </div>
      
  </div>
</template>

<script>

export default {
  name: "FooterComponentIndex",
  data: function(){
      return{
          comicsLinks:[
              {
                  text:"Character",
                  url:"#",
                  current: false,
              },
              {
                  text:"Comics",
                  url:"#",
                  current: false,
              },
              {
                  text:"Movies",
                  url:"#",
                  current: false,
              },
              {
                  text:"TV",
                  url:"#",
                  current: false,
              },
              {
                  text:"Games",
                  url:"#",
                  current: false,
              },
              {
                  text:"Videos",
                  url:"#",
                  current: false,
              },
              {
                  text:"News",
                  url:"#",
                  current: false,
              },
          ],

          dcLinks:[
              {
                  text:"Terms of use",
                  url:"#",
                  current: false,
              },
              {
                  text:"Privacy policy (New)",
                  url:"#",
                  current: false,
              },
              {
                  text:"Add choices",
                  url:"#",
                  current: false,
              },
              {
                  text:"Advertising",
                  url:"#",
                  current: false,
              },
              {
                  text:"Job",
                  url:"#",
                  current: false,
              },
              {
                  text:"Subscriptions",
                  url:"#",
                  current: false,
              },
              {
                  text:"Talent Workshops",
                  url:"#",
                  current: false,
              },
              {
                  text:"CPSC Certificate",
                  url:"#",
                  current: false,
              },
              {
                  text:"Ratings",
                  url:"#",
                  current: false,
              },
              {
                  text:"Shop help",
                  url:"#",
                  current: false,
              },
              {
                  text:"Contact US",
                  url:"#",
                  current: false,
              },
          ],
          sitesLinks:[
               {
                  text:"DC",
                  url:"#",
                  current: false,
              },
               {
                  text:"MAD Magazine",
                  url:"#",
                  current: false,
              },
               {
                  text:"DC Kids",
                  url:"#",
                  current: false,
              },
               {
                  text:"DC Universe",
                  url:"#",
                  current: false,
              },
               {
                  text:"DCmpower Visa",
                  url:"#",
                  current: false,
              },
          ],
          shopLinks:[
               {
                  text:"Shop DC",
                  url:"#",
                  current: false,
              },
               {
                  text:"Shop DC Collectibles",
                  url:"#",
                  current: false,
              },
          ]
      }
  }
};

</script>

<style lang="scss" scoped>

    #my-container{
        background-image: url("../assets/img/footer-bg.jpg");
    }

    #lists-footer-container{
        width: 70%;
        margin: 0 auto;
        height: 450px;
        display: flex;
        justify-content: space-between;
        align-items: center;

            #links-footer{
                display: flex;
                justify-content: center;
                color: white;
                width: 50%;
                  
                    .link{
                        display: flex;
                        flex-direction: column;
                        align-items: center;
                        width: 25%;

                        h4{
                            font-size: 1.4rem;
                            font-weight: 800;
                        }
                        ul{
                            
                            li{
                            list-style: none;
                            padding: .2rem;
                            
                            
                               a{
                                   text-decoration: none;
                                   color: lightgrey;
                                   font-size: 1rem;
                                   margin-bottom: .2rem;
                                   

                                   &:hover{
                                       color: white;
                                   }
                               }
                            }
                        }
                        
                        
                    }
            }

            #bg-container{

                width: 50%;
                height: 100%;
                

                    #img-footer{
                    width: 100%;
                    height: 100%;
                    background-image: url("../assets/img/dc-logo-bg.png");
                    background-size: cover;
                    background-position: center;
                    
                    }
            }        
    }
    #grey-container{
        background-color: rgb(145, 145, 145);
    }
    #my-btn{

        border: solid 2px rgb(4, 84, 189);
        padding: 8px;
        margin-left: 20px;
        a{
            text-decoration: none;
            color: white;
        }
    }

    #social-footer-container{
        width: 70%;
        margin: 0 auto;
        height: 100px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    #icons-social-container{
        display: flex;
        justify-content: center;
        align-items: center;
        margin-right: 20px;
        color: rgb(4, 84, 189);

        .social-icon{
            margin-left: 1rem;
        }
    }
    
</style>