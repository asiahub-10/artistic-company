<template>
  <div id="app">
    <my-header/>
    <intro/>
    <about/>
    <course/>
    <sale-point/>
    <news/>
    <contact/>
    <my-footer/>
    <!--<div class="my-5 py-5"></div>-->
  </div>
</template>

<script>
import Header from './components/Header'
import Intro from './components/Intro'
import About from './components/About'
import Course from './components/Course'
import SalePoint from './components/SalePoint'
import News from './components/News'
import Contact from './components/Contact'
import Footer from './components/Footer'

export default {
  name: 'app',
  components: {
    'my-header': Header,
    'intro': Intro,
    'about': About,
    'course': Course,
    'sale-point': SalePoint,
    'news': News,
    'contact': Contact,
    'my-footer': Footer
  },
  data () {
    return {

    }
  }
}
</script>

<style>
  body
  {
    font-family: Poppins;
  }

  @font-face
  {
    src: url("/../static/fonts/Poppins/POPPINS-REGULAR.TTF");
    font-family: Poppins;
  }
  .header-font
  {
    font-family: Gabriola;
    font-size: 50px;
  }
  .align-center
  {
    align-items: center;
  }

</style>
