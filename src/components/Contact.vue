<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <h1 class="header-font font-weight-bold text-info text-center my-5">Contacto</h1>
        </div>
        <div class="col-lg-4 col-sm-6 mx-auto pb-4">
          <div class="card card-body text-center border-0 shadow">
            <i class="fab fa-whatsapp mx-auto mb-4 fa-3x text-info"></i>
            <h5>0-000-0000</h5>
          </div>
        </div>
        <div class="col-lg-4 col-sm-6 mx-auto pb-4">
          <div class="card card-body text-center border-0 shadow">
            <i class="far fa-envelope mx-auto mb-4 fa-3x text-info"></i>
            <h5>xzy@gmail.com</h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Contact"
}
</script>

<style scoped>
  .shadow {
    box-shadow: 0 0.25rem 1rem rgba(23, 162, 184, .4) !important;
  }
</style>
