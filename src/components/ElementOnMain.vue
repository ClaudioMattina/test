<template>
  

         <div class="my-scheda">
            <div class="img-scheda-container">
              <img :src="imgUrl" :alt="serieTitle">
            </div>
            <h3> {{serieTitle}} </h3>
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
              width: calc(76% / 6);
              height: 100%;
              /* background-color: aqua; */
              flex-direction: column;
              display: flex;
              padding: 1%;
              
              

              h3{
                font-size: 1rem;             
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