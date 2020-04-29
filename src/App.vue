<template>
  <div class="app">
    <Navbar></Navbar>
    <!--router-link to="/Home">About</router-link-->
    <!--router-link to="/about">About</router-link-->
    <div class="block"></div>
    <router-view/>
    <Footer></Footer>
  </div>
</template>

<script>
  import Navbar from './components/Header/Navbar.vue'
  import Footer from './components/Footer/Footer.vue'
  export default{
    components:{
      Navbar,
      Footer
    }
  }
</script>

<style>
@font-face {/*подключение шрифтов*/
    font-family: 'Font Awesome 5 Free';
    font-style: normal;
    font-weight: 400;
    font-display: block;
    src: url("./components/fonts/fontawesome-free-5.13.0-web/webfonts/fa-regular-400.eot");
    src: url("./components/fonts/fontawesome-free-5.13.0-web/webfonts/fa-regular-400.eot?#iefix") format("embedded-opentype"), url("./components/fonts/fontawesome-free-5.13.0-web/webfonts/fa-regular-400.woff2") format("woff2"), url("./components/fonts/fontawesome-free-5.13.0-web/webfonts/fa-regular-400.woff") format("woff"), url("./components/fonts/fontawesome-free-5.13.0-web/webfonts/fa-regular-400.ttf") format("truetype"), url("./components/fonts/fontawesome-free-5.13.0-web/webfonts/fa-regular-400.svg#fontawesome") format("svg"); }
  
  .far {
    font-family: 'Font Awesome 5 Free';
    font-weight: 400; 
}
@font-face{/*подключение шрифтов*/
    font-family: 'RobotoSlab';
    src: url("./components/fonts/robotoslab/RobotoSlab-Regular.ttf");
}
@font-face {
	font-family: 'Oswald DemiBold';
	src: url('./components/fonts/e0f79531a9eb181d09140c8e33656263/fonts/oswald_demibold.eot?#iefix') format('embedded-opentype'), /* IE < 9 */
		url('./components/fonts/e0f79531a9eb181d09140c8e33656263/fonts/oswald_demibold.woff2') format('woff2'), /* Super Modern Browsers */
		url('./components/fonts/e0f79531a9eb181d09140c8e33656263/fonts/oswald_demibold.woff') format('woff'), /* Firefox >= 3.6, any other modern browser */
		url('./components/fonts/e0f79531a9eb181d09140c8e33656263/fonts/oswald_demibold.ttf') format('truetype'), /* Safari, Android, iOS */
        url('./components/fonts/e0f79531a9eb181d09140c8e33656263/fonts/oswald_demibold.svg#oswald_demibold') format('svg'); /* Chrome < 4, Legacy iOS */
}
.app{
  width: 100%;
  height: 100%;
  min-width: 1140px;
  position: relative;
}
.block{
  height: 1500px;
  width: 100%;
}
</style>
