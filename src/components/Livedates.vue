<template>
  <div class="bg-color">
    <div class="container mt-5 color-text">
                <div class="row">
                    <div class="col-12 bg-text " >
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