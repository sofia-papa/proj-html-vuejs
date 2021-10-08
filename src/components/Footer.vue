<template>
  <div class="bg-footer bg-dark">
    <div class="footer-logo px-5 py-5 d-flex justify-content-around">
      <img class="avada-music-logo " src="../assets/avada-music-logo.png" alt="">
    
    <nav class="link-elements">
      <ul class="">
        <li v-for= "(link, index) in links" :key= "index"><a :class= "{ active : link.current}"> {{ link.text }}</a></li>
      </ul>
    </nav>
  </div>

  <div class="bg-footer-2 px-2 py-2">
    <div class="d-flex justify-content-between mx-2">
      <p class="my-4">Copyright 2012 - 2020 | AVADA THEME BY THEMEFUSION | ALL RIGHTS RESERVED | POWERED BY WORDPRESS</p>

      <nav>
        <ul class="">
          <li class="bg-dark mx-2 p-2"><i class="fab fa-facebook-f"></i></li>
          <li class="bg-dark mx-2 p-2"><i class="fab fa-twitter"></i></li>
          <li class="bg-dark mx-2 p-2"><i class="fab fa-instagram"></i></li>
          <li class="bg-dark mx-2 p-2"><i class="fab fa-youtube"></i></li>
        </ul>
      </nav>
    </div>
  </div>
</div>

</template>

<script>

export default {
  name: "Footer",
  components:{

  },

  data: function(){
    return {
      links: [
        {
          text: "Home",
          url: "#home"
        },
        {
          text: "Meet The Band",
          url: "#Meet The Band"
        },
        {
          text: "Live Dates",
          url: "#Live Dates"
        },
        {
          text: "Lates News",
          url: "#home"
        },
        {
          text: "Albums",
          url: "#home"
        },
        {
          text: "Fans",
          url: "#home"
        },
      ]
    }
  }

}
</script >

<style lang= "scss">
 

</style>