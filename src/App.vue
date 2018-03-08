<template>
  <div id="app">
    <!-- <header>
      <span>Vue.js PWA</span>
    </header>
    <main>
      <img src="./assets/logo.png" alt="Vue.js PWA">
      <router-view></router-view>
    </main> -->

    <section class="hero is-dark is-fullheight">
      <div class="hero-head">
        <nav class="navbar">
          <div class="container">
            <div class="navbar-brand">
              <a class="navbar-item" href="../">
              <img src="../static/img/it.png" alt="Logo">
            </a>
            <span class="navbar-burger burger" data-target="navbarMenu"
              :class="{'is-active': isActive}" @click="isActive = !isActive">
              <span></span>
              <span></span>
              <span></span>
            </span>
            </div>
            <div id="navbarMenu" class="navbar-menu" :class="{'is-active': isActive}">
            <div class="navbar-end">
              <router-link to="/" class="navbar-item" active-class="is-active">
                Домашня сторінка
              </router-link>
              <!-- <router-link to="/projects" class="navbar-item">
                Проекти
              </router-link>
              <router-link to="/fotos" class="navbar-item">
                Фото
              </router-link> -->
              <span class="navbar-item">
                <a class="button is-white is-outlined is-small" href="https://www.facebook.com/CoWorking.Shostka/">
                  <span class="icon">
                    <img src="../static/img/facebook.svg"/>
                  </span>
                  <span>Facebook</span>
                </a>
              </span>
            </div>
            </div>
          </div>
        </nav>
      </div>

      <router-view></router-view>
    </section>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {isActive: false}
  }
}
</script>

<style>
body {
  margin: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: whitesmoke;
}

/* main {
  text-align: center;
  margin-top: 40px;
}

header {
  margin: 0;
  height: 56px;
  padding: 0 16px 0 24px;
  background-color: #35495E;
  color: #ffffff;
}

header span {
  display: block;
  position: relative;
  font-size: 20px;
  line-height: 1;
  letter-spacing: .02em;
  font-weight: 400;
  box-sizing: border-box;
  padding-top: 16px;
} */

.hero.is-dark {
  background: linear-gradient(
      rgba(0, 0, 0, 0.5),
      rgba(0, 0, 0, 0.5)
    ), url('https://unsplash.it/1200/900?image=36') no-repeat center center fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
.hero .nav, .hero.is-success .nav {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.hero .subtitle {
  padding: 3rem 0;
  line-height: 1.5;
}
</style>
