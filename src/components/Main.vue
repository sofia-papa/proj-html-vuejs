<template>
  <div class="">
      <div class="bg-first-main text-center text-white ">
        <div class="row p-5 ">
            <div class="col-12 my-5 ">
                <h1 class="title py-5">Music is Life</h1>
                <hr class="margin-center">
                <p class="subtitle px-5 margin-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      </div>

      <div class="bg-second-main text-center text-white">
        <div class="row">
            <div class="col-12 my-5">
                <h1 class="title py-5">Latest Band News</h1>
                <hr class="margin-center">
                <p class="subtitle px-5 margin-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      
        <div class="container">
            <div class="row">
              <Cardone />
            </div>
        </div>
     </div>

      <div class="red-line text-center text-white">
         <p>View all live dates</p>
      </div>

      <div>
        <Playmusic/>
      </div>

      <div class="bg-second-main text-white ">
        <div class="row text-center">
            <div class="col-12">
                <h1 class="title py-5">Live Dates</h1>
                <hr class="margin-center">
                <p class="subtitle margin-center mb-5">Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga consequuntur quibusdam vero, itaque eveniet recusandae exercitationem iure odit, dolores natus sequi, ipsa laborum tenetur reiciendis eos iusto omnis aliquam obcaecati!</p>
            </div>
        </div>
      <div class="color-text pb-5">
          <Livedates class= "" v-for="(dates, index) in festival" :key= "index" :title= "dates.date"/>
      </div>
      </div>

      <div class="red-line text-center text-white">
         <p>View all live dates</p>
      </div>
    </div>
</template>

<script>
import band from "../data/band.js";
import Playmusic from './Playmusic.vue'
import Livedates from './Livedates.vue'
import dates from "../data/dates.js";
import Cardone from "./Cardone.vue"

export default {
    name: "band",

    components: {
        Playmusic,
        Livedates,
        Cardone,
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

.margin-center{
    margin: 20px 380px;
}

</style>