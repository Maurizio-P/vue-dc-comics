<template>
  <footer>
    <div class="bg-color-blue">
      <div class="container">
        <section class="top-section-blue">
          <!-- qui icone della sezione blu -->
          <div class="card">
            <div class="img-container">
              <img src="../assets/buy-comics-digital-comics.png" alt="" />
            </div>
            <h5>Digital Comics</h5>
          </div>
          <div class="card">
            <div class="img-container">
              <img src="../assets/buy-comics-merchandise.png" alt="" />
            </div>
            <h5>Dc Merchandise</h5>
          </div>
          <div class="card">
            <div class="img-container">
              <img src="../assets/buy-comics-shop-locator.png" alt="" />
            </div>
            <h5>Subscription</h5>
          </div>
          <div class="card">
            <div class="img-container">
              <img src="../assets/buy-comics-subscriptions.png" alt="" />
            </div>
            <h5>Comic shop locator</h5>
          </div>
          <div class="card">
            <div class="img-container">
              <img src="../assets/buy-dc-power-visa.svg" alt="" />
            </div>
            <h5>dc power visa</h5>
          </div>
        </section>
      </div>
    </div>

    <div class="link-container">
        <div class="container">
            <div class="row">

                <div class="col-7">
                    <div class="col-4">
                        <ul>
                            <li>Dc comics</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                        </ul>
                        <ul>
                            <li>Shop</li>
                            <li>shop dc</li>
                            <li>shop dc coll</li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <ul>
                            <li>Dc</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                        </ul>
                    </div>
                    <div class="col-4">
                        <ul>
                            <li>Sites</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                            <li>testo</li>
                        </ul>
                    </div>
                </div>
                <div class="img-container">
                    <img src="../assets/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>  
    </div>

    <div class="bg-color-grey">
        <div class="container">
            <section>
                <button class="button-footer"><a class="sign-up" href="">sign-up now</a></button>
                <div class="link-social">
                    <h5 class="follow">follow us</h5>
                    <div class="social">
                        <img src="../assets/footer-facebook.png" alt="">
                        <img src="../assets/footer-twitter.png" alt="">
                        <img src="../assets/footer-youtube.png" alt="">
                        <img src="../assets/footer-pinterest.png" alt="">
                        <img src="../assets/footer-periscope.png" alt="">
                    </div>
                </div>
            </section>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss">
@import "../styles/variables";

footer {
  background-image: url("../assets/footer-bg.jpg");
  padding-top: calc($paddingY * 2);
  position: relative;
  overflow: hidden;

  .bg-color-blue {
    background-color: #0282f9;
    padding: ($paddingY * 2) 0;
    position: absolute;
    top: 0;
    left: 0;
    right: 0;

    section {
      display: flex;
      justify-content: space-between;

      .card {
        display: flex;
        align-items: center;

        .img-container {
          width: 40px;
          display: inline-block;

          img {
            width: 100%;
          }
        }

        h5 {
          display: inline-block;
          margin-left: 10px;
          text-transform: uppercase;
          font-weight: lighter;
          color: white;
        }
      }
    }
  }

    .link-container{
        padding-top: calc(122px + $paddingY);
        padding-bottom: calc($paddingY * 2);

        .col-7{
            display: flex;

            .col-4 {
                margin-right: 15px;
                ul{
                    list-style: none;
                    padding: 0;
                    margin: 0;

                    li{
                        color: #78797b;
                    }
                    
                    li:first-child {
                        color: white;
                        font-size: 20px;
                        margin: 10px 0;
                        text-transform: uppercase;
                    }

                }
            }
        }

        .img-container{
            position: absolute;
            right: 200px;
            top: 10px;
        }
    }

    .bg-color-grey{
        background-color: #303030;
        padding: calc($paddingY * 2) 0;
        position: relative;
        z-index: 1;

        section{
            display: flex;
            justify-content: space-between;

            .button-footer{
                background-color: rgba($color: #000000, $alpha: 0);
                border: 1px solid lightskyblue;
                padding: 15px 10px;

                a{
                    text-decoration: none;
                    color: white;
                    text-transform: uppercase;
                }
            }

            .link-social {
                display: flex;
                align-items: center;

                .follow{
                    text-transform: uppercase;
                    color: #1385ff;
                    margin-right: 20px;
                }

                .social {
                    img{
                        margin-left: 10px;
                    }
                }
            }


        }

    }
}

.row{
    display: flex;
}

.col-4{
    width: calc(100% / 12 * 4);
}

.col-5{
    width: calc(100% / 12 * 5);
}

.col-7 {
    width: calc(100% / 12 * 7);
}
</style>