<template lang="">
    <div class="container-main">
        <section class="container-header-main">
            <div class="content-header-main">
                <div class="jumbotron"></div>
            </div>
        </section>
        <section class="container-main-main">
            <div class="container-main-card">
                <CardElement v-for="card in comicCards"
                    :img="card.thumb"
                    :serie="card.series"
                />
            </div>
        </section>
        <section class="container-footer-main">
            <div class="container-footer-main-cards">
                <div class="footer-main-card">
                    <img class="img-footer-main" src="../assets/img/img/buy-comics-digital-comics.png" alt="">
                    <p>digital comics</p>
                </div>
                <div class="footer-main-card">
                    <img class="img-footer-main" src="../assets/img/img/buy-comics-merchandise.png" alt="">
                    <p>dc merchandise</p>
                </div>
                <div class="footer-main-card">
                    <img class="img-footer-main" src="../assets/img/img/buy-comics-subscriptions.png" alt="">
                    <p>subscription</p>
                </div>
                <div class="footer-main-card">
                    <img class="img-footer-main" src="../assets/img/img/buy-comics-shop-locator.png" alt="">
                    <p>comic shop locator</p>
                </div>
                <div class="footer-main-card">
                    <img class="img-footer-main" src="../assets/img/img/buy-dc-power-visa.svg" alt="">
                    <p>dc power visa</p>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
import CardElement from './CardElement.vue';

export default {
    name: 'AppMain',
    data() {
        return {
            comicCards: [
          {
              "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
              "price": "$19.99",
              "series": "Action Comics",
              "type": "comic book",
          },
          {
              "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
              "price": "$3.99",
              "series": "American Vampire 1976",
              "type": "comic book",
          },
          {
              "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
              "price": "$16.99",
              "series": "Aquaman",
              "type": "graphic novel",
          },
          {
              "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
              "price": "$2.99",
              "series": "Batgirl",
              "type": "comic book",
          },
          {
              "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
              "price": "$3.99",
              "series": "Batman",
              "type": "comic book",
          },
          {
              "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
              "price": "$2.99",
              "series": "Batman Beyond",
              "type": "comic book",
          },
          {
              "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
              "price": "$3.99",
              "series": "Batman/Superman",
              "type": "comic book",
          },
          {
              "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
              "price": "$4.99",
              "series": "Batman/Superman Annual",
              "type": "comic book",
          },
          {
              "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
              "price": "$5.99",
              "series": "Batman: The Joker War Zone",
              "type": "comic book",
          },
          {
              "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
              "price": "$6.99",
              "series": "Batman: Three Jokers",
              "type": "comic book",
          },
          {
              "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
              "price": "$4.99",
              "series": "Batman: White Knight Presents: Harley Quinn",
              "type": "comic book",
          },
          {
              "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
              "price": "$16.99",
              "series": "Catwoman",
              "type": "graphic novel",
          },
            ]

        }
    },
    components: {
        CardElement
    }

}

</script>

<style lang="scss" scoped>
@use '../styles/partials/mixins.scss' as *;

.container-main{
  width: 100%;
}

.container-header-main{
  width: 100%;
  background-color: #1c1c1c;
}

.content-header-main{
  width: 100%;
  height: 350px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  color: white;
  font-size: 1rem;
  font-weight: bolder;
}

.jumbotron{
  width: 100%;
  height: 100%;
  background-image: url(../assets/img/img/jumbotron.jpg);
  background-position: top;
  background-size: cover;
}

.container-main-main{
  width: 100%;
  height: 550px;
  background-color: #1c1c1c;
  margin: 0 auto;
  @include flex(row, center, center);
}

.container-main-card{
    width: 70%;
    @include flex(row, space-evenly, center);
    flex-wrap: wrap;
}

.container-footer-main{
  width: 100%;
  background-color: #0282F9;
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  z-index: 1;
}

.container-footer-main-cards{
  width: 65%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer-main-card{
  width: 20%;
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer-main-card p{
  text-transform: uppercase;
  font-size: .7rem;
  color: white;
  margin-left: .5rem;
}

.img-footer-main{
  width: 40px;
  height: 50px;
}
</style>