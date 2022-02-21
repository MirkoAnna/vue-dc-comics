<template>

  <div class="header-container">
      <div id="logo">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
  </div>

</template>


<script>
export default {
  name: 'HeaderComponent',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import "../assets/style/variables.scss";

    .header-container {
        width: 100%;
        height: 15vh;
        background-color: $headerBackground;
    }

</style>