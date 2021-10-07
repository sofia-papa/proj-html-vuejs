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
          <Card />
      </div>
  </div>
</template>

<script>
import band from "../data/band.js"
import Card from './Card.vue'

export default {
    name: "band",

    components: {
        Card,
    },
    data: function() {
        return {
            products: band,
        }
    }

}
</script >

<style lang="scss">


</style>