<template>
    <div class="main-bottom-container">
        <ul>
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <a href="#">DIGITAL COMICS</a>
            </li>

            <li>
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                <a href="#">DC MERCHANDISE</a>
            </li>

            <li>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                <a href="#">SUBSCRIPTION</a>
            </li>

            <li>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <a href="">COMIC SHOP LOCATOR</a>
            </li>

            <li>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                <a href="">DC POWER VISA</a>
            </li>

        </ul>
    </div>
</template>


<script>
export default {
  name: 'MainBottom',
  data() {
      return {
          buyComics: [
              {
                  "icon": "../assets/img/buy-comics-digital-comics.png",
                  "text": "DIGITAL COMICS"
              },
              {
                  "icon": "../assets/img/buy-comics-digital-comics.png",
                  "text": "DC MERCHANDISE"
              },
              {
                  "icon": "../assets/img/buy-comics-digital-comics.png",
                  "text": "SUBSCRIPTION"
              },
              {
                  "icon": "../assets/img/buy-comics-digital-comics.png",
                  "text": "COMIC SHOP LOCATOR"
              },
              {
                  "icon": "../assets/img/buy-comics-digital-comics.png",
                  "text": "DC POWER VISA"
              },
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
        display: flex;
        justify-content: space-around;
        width: 100%;
        height: 19vh;
        font-size: $sizeBasic;
        background-color: $mainBottomBackground;
        color: $headerBackground;

        

        ul {
            width: 100%;
            display: flex;
            justify-content: center;

            li {
                width: calc(65% / 5);
                margin: 0 1%;
                display: flex;
                align-items: center;


                img {
                    width: 2rem;
                    height: 2.5rem;
                }

                a {
                    margin: 0 5%;
                    text-decoration: none;
                    color: $headerBackground;
                }
            }
        }
    }

</style>