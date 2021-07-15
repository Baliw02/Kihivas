<template>

<div id="app">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap" rel="stylesheet"> 

  <div v-if="window.width > 1054" class="nav">
    <Header ></Header>
  </div>
  <div v-if="window.width <= 1054" class="side">
    <Sidebar ></Sidebar>
  </div>
  <div class="content">
    <FirstContent></FirstContent>
  </div>
  <div class="section">
    <SectionOne></SectionOne>
  </div>
  <div class="sectiontwo">
    <SectionTwo></SectionTwo>
  </div>
  <div>
    <SectionThree></SectionThree>
  </div>
  <div class="gallery">
    <Chooser></Chooser>
  </div>
  <div class="products">
    <Products></Products>
  </div>
</div>
</template>

<script>
import Header from './components/Header'
import FirstContent from './components/FirstContent'
import SectionOne from './components/Section'
import SectionTwo from './components/Sectiontwo'
import SectionThree from './components/Sectionthree'
import Chooser from './components/Chooser'
import Sidebar from './components/Sidebar'
import Products from './components/Products'


export default {
  name: 'App',
  components: {
    Header,
    FirstContent,
    SectionOne,
    SectionTwo,
    SectionThree,
    Chooser,
    Sidebar,
    Products
  },
  created() {
    window.addEventListener('resize', this.handleResize);
    this.handleResize();
    },
  data(){
    return{
      window:{
        width:0
      }
    }
  },
  methods:{
    handleResize(){
      this.window.width = window.innerWidth
    }
  }
}
</script>

<style lang="scss">
$sec: rgba(72, 61, 139, 100%);
$prim: white;


.side{
  z-index: 999;
  padding:10px 10px;
  display: block;
  background-color: black;
  width: 100%;
  height: fit-content;
  position: fixed;
  right: 0;
}
.nav{
  width:100%;
  min-height: 100px;

}
.content{
  align-items: center;
  height: 650px;
}
.gallery{
  margin-top: 20%;
}
h1{
  font-family: Roboto;
  font-weight: 300;
}
body{
  text-align: center;
  margin:0;
  overflow-x: hidden;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
