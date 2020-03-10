<template>
  <div>
    <footer>
      <div class="border-top mt-5 py-5">
        <div class="container">
          <div class="row">
            <div class="col-sm-12">
              <h1 class="text-info header-font text-center mb-3">Newsletter</h1>
            </div>
            <div class="col-xl-5 col-lg-6 col-md-8 col-sm-10 mx-auto">
              <div class="input-group">
                <input type="text" class="form-control shadow-none" placeholder="Email address" aria-label="Recipient's username" aria-describedby="basic-addon2">
                <div class="input-group-append">
                  <button class="btn btn-info  shadow-none" type="button"><i class="fab fa-telegram-plane mx-3 btn-icon"></i></button>
                </div>
              </div>
            </div>
            <div class="col-sm-12">
              <h1 class="text-info header-font text-center mt-5 mb-3">Follow Us</h1>
            </div>
            <div class="col-xl-5 col-lg-6 col-md-8 col-sm-10 mb-3 mx-auto text-center">
              <a href="" class="btn btn-info mx-2 btn-lg text-uppercase" target="_blank" title="Follow on Facebook"><i class="fab fa-facebook-square mr-2"></i> Facebook</a>
              <a href="" class="btn btn-info mx-2 btn-lg text-uppercase" target="_blank" title="Follow on Instragram"><i class="fab fa-instagram mr-2"></i> Instragram</a>
            </div>
          </div>
        </div>
      </div>
      <div class="bg-info">
        <p class="text-white text-center mb-0 py-3">Copyright © 2020 Asia R. | Designed by <span class="font-weight-bold font-italic">Asia R.</span></p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>
.border-top
{
  border-top: 5px solid #17a2b8 !important;
  background: #f7f7f7;
}
  input
  {
    border: 1px solid #17a2b8;
  }
  .btn-icon
  {
    font-size: 18px;
  }
</style>
