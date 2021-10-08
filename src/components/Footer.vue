<template>
  <div class="bg-footer bg-dark ">
    <div class="footer-logo px-5 py-5 d-flex justify-content-around">
      <img class="avada-music-logo " src="../assets/avada-music-logo.png" alt="">
    
    <nav class="link-elements">
      <ul class="">
        <li v-for= "(link, index) in links" :key= "index"><a :class= "{ active : link.current}"> {{ link.text }}</a></li>
      </ul>
    </nav>
  </div>
</div>
</template>

<script>
export default {
  name: "Footer",

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