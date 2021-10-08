<template>
  <div class="header-container header-wrapper">
      <div class="container-fluid">
          <div class="row">
              <div class="col-12 d-flex justify-content-between">
                  <img src="../assets/logo_footer.png" alt="" class="float-left m-3 p-3 d-flex" >
                  <div class="pos-f-t m-3 p-3">
                        <div class="collapse" id="navbarToggleExternalContent" >
                            <div class=" p-4">
                            <h4 class="text-white">Collapsed content</h4>
                            <span class="text-muted">Toggleable via the navbar brand.</span>
                            </div>
                        </div>
                        <nav class="navbar navbar-dark justify-content-end">
                            <button class="navbar-toggler " type="button" data-toggle="collapse" data-target="#navbarToggleExternalContent" 
                            aria-controls="navbarToggleExternalContent" aria-expanded="false" aria-label="Toggle navigation">
                            <span class="navbar-toggler-icon"></span>
                            </button>
                        </nav>
                    </div>
              </div>
          </div>
      </div>
      
        <div class="container text-center text-white mt-5">
            <div class="row">
                <div class="col-12">
                    <h1 class="title">Untold Stories</h1>
                    <p class="subtitle">There is an untold story behind every favorite song.</p>
                    <button type="button" class="btn btn-outline-danger my-5 mx-3">LATEST ALBUM</button>
                    <button type="button" class="btn btn-outline-danger">LIVE DATES</button>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../style/variable.scss';
@import '../style/general.scss';

.header-wrapper{
    height: 100vh;
    width: 100%;
    background-image: url("../assets/home_slider.jpg");
}

h1.title {
    font-family: $fontTitle;
    font-size: 8rem;
}

p.subtitle {
    font-family: $fontSubtitle;
    font-size: 2rem;
}

</style>