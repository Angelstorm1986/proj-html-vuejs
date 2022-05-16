<template>
  <div class="container-jumbo">
      <img src="../assets/images/construction_thumbnail.jpg" alt="Construction">
  </div>
</template>

<script>
export default {
    name: 'AppJumbotron'
}
</script>

<style lang="scss">
@import '../style/vars';
.container-jumbo{
    width: 100%;
    height: 100vh;
    img{
        width: 100%;
        height: 100%;
    }
}
</style>