<template>
  <section class="cards-margin"> 
      <div class="container">
       <div class="row">
           <div class="col-lg-2 col-md-4 col-6 album me-4">
                    <h5 class="title-series">{{ title }}</h5>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
 name: "card",
    props: {

        title: {
            String,
            required: true,
        },
        src: String, 
    },
    description: String,

    

}
</script>

<style>

</style>