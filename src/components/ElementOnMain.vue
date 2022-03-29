<template>
  <div>
         <div class="my-scheda">
            <div class="img-scheda-container">
              <img :src="imgUrl" :alt="serieTitle">
            </div>
            <h3> {{serieTitle}} </h3>
        </div>
  </div>
</template>

<script>
export default {
    name: "MainElement",
    props:['imgUrl','serieTitle']
}
</script>

<style lang="scss" scoped>
     .my-scheda{
              width: calc(100% / 6);
              height: 100%;
              background-color: aqua;
              flex-direction: column;
              display: flex;

              h3{
                font-size: .2rem;
                
              }
              

              .img-scheda-container{
                width: 100%;
                height: 100%;

                img{
                  width: 100%;
                  height: 100%;
                }
              }
     }
</style>