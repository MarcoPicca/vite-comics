<template lang="">
    <section class="container-header-footer">
        <div class="container-content-header-footer">
            <div class="column-header-footer">
                <h3 class="title-content-footer">DC COMICS</h3>
                <ul class="footer-list">
                    <li class="list-footer">Characters</li>
                    <li class="list-footer">Comics</li>
                    <li class="list-footer">Movie</li>
                    <li class="list-footer">Tv</li>
                    <li class="list-footer">Games</li>
                    <li class="list-footer">Videos</li>
                    <li class="list-footer">News</li>
                </ul>
                <h3 class="title-content-footer">SHOP</h3>
                <ul class="footer-list">
                    <li class="list-footer">Shop DC</li>
                    <li class="list-footer">Shop DC Collectibles</li>
                </ul>
            </div>
            <div class="column-header-footer">
                <h3 class="title-content-footer">DC</h3>
                <ul class="footer-list">
                    <li class="list-footer">Terms Of Use</li>
                    <li class="list-footer">Privacy policy (New)</li>
                    <li class="list-footer">Ad Choices</li>
                    <li class="list-footer">Advertising</li>
                    <li class="list-footer">Jobs</li>
                    <li class="list-footer">Sbscriptions</li>
                    <li class="list-footer">Talent Workshops</li>
                    <li class="list-footer">CPSC Certificates</li>
                    <li class="list-footer">Ratings</li>
                    <li class="list-footer">Shop Help</li>
                    <li class="list-footer">Contact Us</li>
                </ul>
            </div>
            <div class="column-header-footer">
                <h3 class="title-content-footer">SITES</h3>
                <ul class="footer-list">
                    <li class="list-footer">DC</li>
                    <li class="list-footer">MAD Magazine</li>
                    <li class="list-footer">DC Kids</li>
                    <li class="list-footer">DC Universe</li>
                    <li class="list-footer">DC Power Visa</li>
                </ul>
            </div>
        </div>
        <div class="mega-icon">
            <img class="mega-icon-bg" src="../assets/img/img/dc-logo-bg.png" alt="">
        </div>
    </section>
    <section class="container-footer-footer">
        <div class="container-content-footer-footer">
            <button class="btn-footer" type="button">sign-up now!</button>
            <div class="container-icon-footer">
                <div class="container-text-icon">
                    <h3 class="title-icon-footer">Follow us</h3>
                </div>
                <div class="container-icon">
                    <img class="icon-footer" src="../assets/img/img/footer-facebook.png" alt="">
                </div>
                <div class="container-icon">
                    <img class="icon-footer" src="../assets/img/img/footer-twitter.png" alt="">
                </div>
                <div class="container-icon">
                    <img class="icon-footer" src="../assets/img/img/footer-youtube.png" alt="">
                </div>
                <div class="container-icon">
                    <img class="icon-footer" src="../assets/img/img/footer-pinterest.png" alt="">
                </div>
                <div class="container-icon">
                    <img class="icon-footer" src="../assets/img/img/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'AppFooter',
}
</script>

<style lang="scss" scoped>
.container-header-footer{
  width: 100%;
  background-image: url(../assets/img/img/footer-bg.jpg);
  background-size: cover;
  background-position: center;
  display: flex;
  justify-content: center;
  
}

.container-content-header-footer{
  width: 70%;
  height: 100%;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.column-header-footer{
  width: 13%;
  height: 350px;
}

.title-content-footer{
  color: white;
  font-weight: lighter;
  padding-top: 2rem;
  margin-bottom: .7rem;
}

.footer-list{
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  font-size: .8rem;
}

.list-footer{
  width: 100%;
  height: 18px;
  color: gray;
  display: flex;
  justify-content: flex-start;
}

.mega-icon-bg{
  width: 500px;
  height: 500px;
  position: absolute;
  top: 1000px;
  right: 230px;
}

.container-footer-footer{
  width: 100%;
  height: 87px;
  background-color: #303030;
  position: relative;
  z-index: 0;
}

.container-content-footer-footer{
  width: 63%;
  height: 100%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.btn-footer{
  width: 130px;
  height: 45px;
  text-transform: uppercase;
  background-color: #303030;
  color: white;
  border: 2px solid #195994;
}

.container-icon-footer{
  width: 35%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.container-text-icon{
  width: 25%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: .6rem;
}

.title-icon-footer{
  text-transform: uppercase;
  color: #026EB1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.container-icon{
  width: calc(75% / 5);
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.icon-footer{
  width: 25px;
  height: 25px;
}
</style>