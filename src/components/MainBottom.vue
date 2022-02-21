<template>
  <div class="main-bottom-container">
      <div class="align-content">
            <ul class="box-shop">

                <li>
                    <div>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="">

                    </div>
                    <span>DIGITAL COMICS</span>
                </li>

                <li>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    <span>DC MERCHANDISE</span>
                </li>

                <li>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </li>

                <li>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <span><a href="">COMIC SHOP LOCATOR</a></span>
                </li>

                <li>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <span><a href="">DC POWER VISA</a></span>
                </li>

            </ul>
      </div>
  </div>
</template>


<script>
export default {
  name: 'MainBottom',
  data() {
      return {
          buyComics: [
              {

              }
          ]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/style/variables.scss";
@import "../assets/style/general.scss";

    .main-bottom-container {
        width: 100%;
        height: 19vh;
        font-size: $sizeBasic;
        background-color: $mainBottomBackground;
        color: $headerBackground;

        .align-content {
            display: flex;

            ul {
                display: flex;
                justify-content: space-around;

                li {
                    display: flex;
                    justify-content: space-around;
                    align-items: center;
                    margin: 0 3%;

                    img {
                        width: 2.5rem;
                        height: 2.5rem;
                    }

                    span {
                        margin: 0 5%;
                    }
                }
            }
        }
    }

</style>