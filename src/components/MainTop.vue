<template>

  <div class="main-top-container">
      <div class="align-content">
          <h2>Content goes here</h2>
      </div>
  </div>

</template>


<script>
export default {
  name: 'MainTop',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import "../assets/style/variables.scss";
    @import "../assets/style/general.scss";

    .main-top-container {
        display: flex;
        align-content: center;
        width: 100%;
        height: 13vh;
        background-color: $mainTopBackground;

        .align-content {
            display: flex;
            align-items: center;
            color: $headerBackground;
        }
    }

</style>