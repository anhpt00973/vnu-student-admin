<template>
  <v-app>
    <Drawer></Drawer>
    <AppBar></AppBar>
    <v-main>
      <div class="container wrap-content-page">
        <v-card
          class="mx-auto pa-5" style="padding-bottom: 40px !important;"
          flat
        >
          <router-view></router-view>
        </v-card>
      </div>
      <Footer></Footer>
    </v-main>
    
  </v-app>
</template>

<script>
import Drawer from '../containerComponents/Drawer'
import AppBar from '../containerComponents/AppBar'
import Footer from '../containerComponents/Footer'
export default {
  name: 'Home',

  components: {
    Drawer,
    AppBar,
    Footer
  },

  data: () => ({
    //
  }),
  created () {
    // let router = this.$router.history.current
    // if (router.path === '/') {
    //   this.$router.push({ path: '/login' })
    // }
  }
};
</script>
<style lang="scss">
  main.v-main {
    padding-top: 54px !important
  }
  @media screen and (max-width: 426px){
    
  }
  @media screen and (max-width: 769px){
    .wrap-content-page {
      padding-bottom: 70px !important
    }
  }
  @media screen and (max-width: 1025px){
    .wrap-content-page {
      padding-bottom: 70px !important
    }
  }
</style>
