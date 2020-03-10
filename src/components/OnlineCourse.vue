<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-sm-12 my-5">
          <h2 class="text-center mb-5 text-info">Online Courses</h2>
          <p class="text-center">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Aperiam atque eius est eveniet magnam. Adipisci aliquid, aspernatur, enim facilis in ipsa ipsam mollitia, nobis nulla quis quisquam ratione recusandae rerum?</p>
        </div>
        <div class="col-sm-12">
          <div class="row">
            <div class="col-lg-8 col-md-7">
              <div class="card border-0">
                <img src="../../static/images/IMG_7388.jpg" alt="Video" class="card-img p-3 video-thumbnail-1"/>
                <div class="card-img-overlay d-flex flex-column justify-content-center">
                  <button type="button" class="btn btn-block bg-transparent shadow-none" data-toggle="modal" data-target="#video1Modal">
                    <i class="fas fa-play text-light fa-3x"></i>
                  </button>
                </div>
              </div>
            </div>
            <div class="col-lg-4 col-md-5">
              <div class="card border-0">
                <img src="../../static/images/IMG_2384.jpg" alt="Video" class="card-img p-3 video-thumbnail-2" />
                <div class="card-img-overlay d-flex flex-column justify-content-center">
                  <button type="button" class="btn btn-block bg-transparent shadow-none" data-toggle="modal" data-target="#video2Modal">
                    <i class="fas fa-play text-light fa-3x"></i>
                  </button>
                </div>
              </div>
              <div class="card border-0">
                <img src="../../static/images/IMG_8707.jpg" alt="Video" class="card-img p-3 video-thumbnail-3" />
                <div class="card-img-overlay d-flex flex-column justify-content-center">
                  <button type="button" class="btn btn-block bg-transparent shadow-none" data-toggle="modal" data-target="#video3Modal">
                    <i class="fas fa-play text-light fa-3x"></i>
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-sm-12 mt-3">
          <div class="text-center bg-info rounded pb-5 mt-5">
            <i class="fab fa-youtube text-info icon"></i>
            <h4 class="text-white mt-4">
              For more tutorials please visit to <a href="" class="font-weight-bold text-light">Tienda Nube</a>.
            </h4>
          </div>
        </div>
      </div>
    </div>
    <!--modal-->
    <div class="modal fade" id="video1Modal" tabindex="-1" role="dialog" aria-labelledby="myLargeModalLabel" aria-hidden="true">
      <div class="modal-dialog modal-dialog-centered modal-lg">
        <div class="modal-content bg-transparent border-0">
          <!-- Modal Header -->
          <div class="modal-header border-bottom-0">
            <button type="button" class="close text-white shadow-none" data-dismiss="modal">&times;</button>
          </div>
          <!-- Modal body -->
          <div class="modal-body videoWrapper">
            <iframe src="https://www.youtube.com/watch?v=pWahNIMRxR0" frameborder="0" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
    <div class="modal fade" id="video2Modal" tabindex="-1" role="dialog" aria-labelledby="myLargeModalLabel" aria-hidden="true">
      <div class="modal-dialog modal-dialog-centered modal-lg">
        <div class="modal-content bg-transparent border-0">
          <!-- Modal Header -->
          <div class="modal-header border-bottom-0">
            <button type="button" class="close text-white shadow-none" data-dismiss="modal">&times;</button>
          </div>
          <!-- Modal body -->
          <div class="modal-body videoWrapper">
            <iframe src="https://www.youtube.com/watch?v=pWahNIMRxR0" frameborder="0" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
    <div class="modal fade" id="video3Modal" tabindex="-1" role="dialog" aria-labelledby="myLargeModalLabel" aria-hidden="true">
      <div class="modal-dialog modal-dialog-centered modal-lg">
        <div class="modal-content bg-transparent border-0">
          <!-- Modal Header -->
          <div class="modal-header border-bottom-0">
            <button type="button" class="close text-white shadow-none" data-dismiss="modal">&times;</button>
          </div>
          <!-- Modal body -->
          <div class="modal-body videoWrapper">
            <iframe src="https://www.youtube.com/watch?v=pWahNIMRxR0" frameborder="0" allowfullscreen></iframe>
          </div>
        </div>
      </div>
    </div>
    <!--modal-->
  </div>
</template>

<script>
    export default {
        name: "OnlineCourse"
    }
</script>

<style scoped>
  .icon
  {
    background: #ffffff;
    height: 100px;
    width: 100px;
    padding: 20px 20px;
    border-radius: 50%;
    border: 5px solid #17a2b8;
    margin-top: -40px;
  }

  .video-title
  {
    border-radius: 0 0 5px 5px;
    border-top: 3px solid #17a2b8;
  }
  .video-img
  {
    border-radius:  5px 5px 0 0;
  }
  .video-thumbnail-1, .video-thumbnail-2, .video-thumbnail-3
  {
    margin-bottom: 20px;
  }
  .card-img
  {
    border: 2px solid #17a2b8;
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
  @media screen and (min-width: 768px) and (max-width: 991.98px)
  {
    .video-thumbnail-1
    {
      height: 300px;
    }
    .video-thumbnail-2, .video-thumbnail-3
    {
      height: 135px;
    }
    .video-thumbnail-2
    {
      margin-bottom: 30px;
    }
  }
  @media screen and (min-width: 992px) and (max-width: 1199.98px)
  {
    .video-thumbnail-2, .video-thumbnail-3
    {
      height: 205px;
    }
    .video-thumbnail-2
    {
      margin-bottom: 30px;
    }
  }
  @media screen and (min-width: 1200px)
  {
    .video-thumbnail-2, .video-thumbnail-3
    {
      height: 245px;
    }
    .video-thumbnail-2
    {
      margin-bottom: 30px;
    }
    .fa-3x
    {
      font-size: 60px;
    }

  }
</style>
