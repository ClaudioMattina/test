<template>

<div class="my-container">
<div id="icones-container">
      <div class="icon">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <h5>DIGITAL COMICS</h5>
      </div>
       <div>
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <h5>DC MERCHANDISE</h5>
      </div>
       <div>
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
          <h5>SUBSCRTIPTIONS</h5>
      </div>
       <div>
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <h5>COMICS SHOP LOCATOR</h5>
      </div>
       <div>
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <h5>DC POWER VISA</h5>
      </div>
      
  </div>
</div>
  
</template>

<script>

export default {
  name: "IconesComponentIndex",
};

</script>

<style lang="scss" scoped>

    .my-container{
        background-color: rgb(4, 84, 189);
    }
    #icones-container{
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        width: 70%;
        margin: 0 auto;
        height: 150px;

        div{
            width: 25%;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 2rem;
            color: white;
            img{
                width: 25%;
                margin-right: 10px;
            }
        }

        
    }
</style>