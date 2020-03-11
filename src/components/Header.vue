<template>
  <div>
    <!--nav-->
    <section>
      <div class="container">
        <div class="row">
          <div class="col-sm-12 text-center">
            <img src="../../static/images/logo.png" alt="Logo" class="mt-4 mb-3" height="70"/>
          </div>
        </div>
        <div class="row">
          <div class="col-sm-12">
            <hr class="bg-info"/>
            <nav class="navbar navbar-expand-md navbar-light">
              <button class="navbar-toggler mx-auto" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>

              <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav mx-auto">
                  <li class="nav-item">
                    <a class="nav-link text-dark font-weight-bold" href="#head">HOME <span class="sr-only">(current)</span></a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link text-dark font-weight-bold" href="#about">SOBRE MI</a>
                  </li>
                  <li class="nav-item dropdown">
                    <a class="nav-link text-dark font-weight-bold dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                      CURSOS
                    </a>
                    <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                      <a class="dropdown-item text-dark font-weight-bold" href="#classCourse">Presenciales</a>
                      <a class="dropdown-item text-dark font-weight-bold" href="#onlineCourse">Online</a>
                    </div>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link text-dark font-weight-bold" href="#salePoint">PUNTOS DE VENTA</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link text-dark font-weight-bold" href="#news">NOVEDADES</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link text-dark font-weight-bold" href="#contact">CONTACTO</a>
                  </li>
                </ul>
              </div>
            </nav>
          </div>
        </div>
      </div>
    </section>
    <!--/.nav-->
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style scoped>
  .nav-item:hover .dropdown-menu
  {
    display: block;
  }
  .dropdown-item:hover
  {
    background: #17a2b8;
    color: #ffffff !important;
  }
</style>
