<template>
  <NavBarVue />
  <router-view />
  <MyFooterVue />
</template>

<script>
import NavBarVue from './components/NavBar.vue';
import MyFooterVue from './components/Footer.vue';

export default {
  components: {
    NavBarVue,
    MyFooterVue,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  size: 16px;
  color:rgb(229, 229, 229);
  font-family: 'Caveat', cursive;
  font-family: 'Pathway Gothic One', sans-serif;
  font-family: 'Sedgwick Ave Display', cursive;
  scroll-behavior: smooth;
}

body{
  // background-image: url(https://i.postimg.cc/YqMy6DH1/pexels-daniel-absi-952670.jpg);
  background-image: url(https://i.postimg.cc/DfDZFDj3/Polish-20230112-223548099.jpg);
}

nav {
  padding: 100px;

  a {
    font-weight: bold;
    color: rgb(226, 226, 226);
    text-decoration: none;

    &.router-link-exact-active {
      color: #42b983;
      text-decoration: none;
    }
  }
}
</style>
