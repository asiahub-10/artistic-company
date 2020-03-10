<template>
  <div>
    <div class="container py-5">
      <div class="row align-center ">
        <div class="col-md-6 mb-4">
          <h1 class="header-font font-weight-bold text-info mb-4">Sobre Mi</h1>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid dolores eum explicabo magnam odit qui quia? A accusantium esse ex excepturi illo in iusto laborum, maxime omnis, quibusdam recusandae velit.</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aliquid dolores eum explicabo magnam odit qui quia? A accusantium esse ex excepturi illo in iusto laborum, maxime omnis, quibusdam recusandae velit.</p>
        </div>
        <div class="col-md-6">
          <div class="card border-0 shadow">
            <img src="../../static/images/video.jpg" alt="Image" class="card-img"/>
            <div class="card-img-overlay text-white d-flex flex-column justify-content-center">
              <button type="button" class="btn btn-block bg-transparent shadow-none" data-toggle="modal" data-target="#aboutModal">
                <i class="far fa-play-circle text-light fa-6x"></i>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!--modal-->
    <div class="modal fade" id="aboutModal" tabindex="-1" role="dialog" aria-labelledby="myLargeModalLabel" aria-hidden="true">
      <div class="modal-dialog modal-dialog-centered modal-lg">
        <div class="modal-content bg-transparent border-0">
          <!-- Modal Header -->
          <div class="modal-header border-bottom-0">
            <button type="button" class="close text-white shadow-none" data-dismiss="modal">&times;</button>
          </div>
          <!-- Modal body -->
          <div class="modal-body videoWrapper">
            <iframe src="../../static/videos/Particles,%20Lights,%20Squares,%20No%20Copyright,%20Copyright%20Free%20Video,%20Motion%20Graphics,%20Background%20Video.mp4" frameborder="0" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
    <!--modal-->
  </div>
</template>

<script>
export default {
  name: "About"
}
</script>

<style scoped>
  .shadow {
    box-shadow: 0 0.25rem 1rem rgba(23, 162, 184, .4) !important;
  }
  .videoWrapper {
    position: relative;
    padding-bottom: 56.25%;
    padding-top: 25px;
    height: 0;
  }
  .videoWrapper iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
</style>
