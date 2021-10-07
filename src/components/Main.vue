<template>
  <div class="bg-first-main">
      <div class="container text-center text-white">
        <div class="row">
            <div class="col-12">
                <h1 class="title">Music is Life</h1>
                <hr>
                <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      </div>

      <div class="container text-center text-white">
        <div class="row">
            <div class="col-12">
                <h1 class="title">Latest Band News</h1>
                <hr>
                <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      </div>
      <div>
          <Card v-for="(band, index) in products" :key= "index" :title= "band.title" :description = "band.description"
             :src= "band.photo"/>
          
      </div>

      <div>
        <Line />
      </div>

      <div>
        <Playmusic/>
      </div>

      <div class="color-text">
          <Livedates v-for="(dates, index) in festival" :key= "index" :title= "dates.date"/>
      </div>
    
  </div>
</template>

<script>
import band from "../data/band.js";
import Card from './Card.vue';
import Line from './Line.vue';
import Playmusic from './Playmusic.vue'
import Livedates from './Livedates.vue'
import dates from "../data/dates.js";

export default {
    name: "band",

    components: {
        Card,
        Line,
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
    background-color: rgb(83, 74, 74) ;
    
}

</style>