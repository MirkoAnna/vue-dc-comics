<template>
      <div class="jumbotron-image">
        <img src="../../assets/img/jumbotron.jpg" alt="">
      </div>
</template>

<script>

export default {
    name: 'MyJumbotron'
}
</script>

<style lang="scss" scoped>

    .jumbotron-image {
        width: 100%;
        height: 38vh;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
</style>