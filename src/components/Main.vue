<template>
  <div class="bg-first-main">
      <div class="container text-center text-white">
        <div class="row ">
            <div class="col-12 my-5">
                <h1 class="title">Music is Life</h1>
                <hr>
                <p class="subtitle px-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      </div>

      <div class="container text-center text-white">
        <div class="row">
            <div class="col-12 my-5">
                <h1 class="title">Latest Band News</h1>
                <hr>
                <p class="subtitle px-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      </div>
      <div>
          <Card v-for="(band, index) in products" :key= "index" :title= "band.title" :description = "band.description"
             :src= "band.photo"/>
      </div>

      <div class="red-line text-center text-white">
         <p>View all live dates</p>
      </div>

      <div>
        <Playmusic/>
      </div>

      <div class="container text-white">
        <div class="row text-center my-5">
            <div class="col-12">
                <h1 class="title">Live Dates</h1>
                <hr>
                <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      <div class="color-text my-5">
          <Livedates v-for="(dates, index) in festival" :key= "index" :title= "dates.date"/>
      </div>
      </div>

      <div class="red-line text-center text-white">
         <p>View all live dates</p>
      </div>
    
  </div>
</template>

<script>
import band from "../data/band.js";
import Card from './Card.vue';
import Playmusic from './Playmusic.vue'
import Livedates from './Livedates.vue'
import dates from "../data/dates.js";

export default {
    name: "band",

    components: {
        Card,
        Playmusic,
        Livedates
    },
    data: function() {
        return {
            products: band,
            festival: dates,
        }
    }

}
</script >

<style lang="scss">

.color-text{
    color: #ea4a56;
    text-transform: uppercase;
}

.bg-text{
    background-color: rgb(68, 67, 67) ;
    
}

.red-line{
    height: 100px;
    background-color: #ea4a56 ;
    text-transform: uppercase;
    padding: 2.5rem;
    font-size: 0.8rem;
}

</style>