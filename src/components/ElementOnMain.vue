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
     
</style>