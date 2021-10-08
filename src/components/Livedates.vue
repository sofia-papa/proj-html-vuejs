<template>
  <div class="bg-color">
    <div class="container mt-1 color-text">
                <div class="row">
                    <div class="col-12 bg-text " >
                        <p class="subtitle my-2"><i class="fas fa-plus mx-2"></i> {{ title }} </p>
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
.subtitle{
    font-size: 0.8rem;
}
</style>