<template>
  <div class="">
    <div class="container text-white mt-5 color-text">
                <div class="row">
                    <div class="col-12 bg-secondary" >
                        <p class="subtitle"><i class="fas fa-plus"></i> {{ title }} </p>
                    </div>
                </div>
            </div>
  </div>
</template>

<script>


export default {

    props: {
        title:{
            String,
        } 
    },
    


}
</script>

<style lang= "scss">

</style>