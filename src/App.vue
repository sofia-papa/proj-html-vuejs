<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import './style/variable.scss';
@import './style/general.scss';
@import '~@fortawesome/fontawesome-free/css/all.css';
#app {

h1.title{
  font-family: $fontTitle;
}

.bg-first-main{
  background-color: $bgsecondmain;
}

ul{
  margin: 25px 0;
  display: flex;
  justify-content: end;
  list-style: none;
  font-family: $fontText;
  padding: 0 2rem;
 
}

li a{
  padding: 20px;
  text-decoration: none;
  color: $bgfirstmain;

  &.active{
    color: gray;
  }

  &:hover{
    background-color: ghostwhite;
  }

}

.bg-footer-2{
  background-color: #2b2b2c;
  font-family:$fontText;
  font-size: 0.8rem;
  color: $bgfirstmain;
}

.red-line{
  font-family: $fontText;
}

.color-text{
  font-family: $fontText;
}

.fas.fa-plus{
  font-size: 5px;
  color: white;
  
}
  
}
</style>
