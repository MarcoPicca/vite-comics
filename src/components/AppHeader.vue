<template lang="">
    <div class="container-header">
        <div class="container-content-header">
            <section class="container-logo">
                <img class="logo" src="../assets/img/img/dc-logo.png" alt="logo DC comics">
            </section>
            <ul class="container-nav-list">
                <li class="nav-list">Characters</li>
                <li class="nav-list">Comics</li>
                <li class="nav-list">Movie</li>
                <li class="nav-list">Tv</li>
                <li class="nav-list">Games</li>
                <li class="nav-list">Collectibles</li>
                <li class="nav-list">Videos</li>
                <li class="nav-list">Fans</li>
                <li class="nav-list">News</li>
                <li class="nav-list">Shop</li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    name: 'AppHeader',
}
</script>

<style lang="scss" scoped>
.container-header{
  width: 100%;
}

.container-content-header{
  width: 63%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.container-logo{
  height: 80px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.logo{
  width: 50px;
  height: 50px;
}

.container-nav-list{
  width: 55%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  list-style-type: none;
}

.nav-list{
  width: calc ((100% / 10) - 1 rem );
  height: 80px;
  text-transform: uppercase;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  font-size: .5rem;
  font-weight: bolder;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>