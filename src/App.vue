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

<style lang="scss" >
@import './style/variable.scss';
@import './style/general.scss';
@import '~@fortawesome/fontawesome-free/css/all.css';
#app {

h1.title{
  font-family: $fontTitle;
}

.bg-first-main{
  background-color: #484852;
}

.bg-second-main{
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
    ;
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

.first-square{
  width: 600px;
}

.album-wrapper{
  width: 300px;
  
  img{
    width: 290px;
  }
}

.height-photo img{
  height: 635px ;
  width: 333.33px;

}

#height-photo-2{
  width: 333.33px;
}
  
.color-text-album{
  color:$lineColor;
  font-family: $fontText;
  font-size: 1.1rem;
  padding-top: 1rem;
}

.font-text-album{
  color: $bgfirstmain;
  font-size: 0.8rem;
  padding: 0 1rem;
}

.jumbo{
   margin: 0 180px;
}
}
</style>
