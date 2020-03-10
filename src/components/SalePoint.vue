<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <h1 class="header-font font-weight-bold text-info text-center my-5">Puntos De Venta</h1>
        </div>
        <div class="col-sm-12">
          <carousel :autoplay="true" :nav="false" :loop="true" :responsive="{0:{items:1}, 700:{items:2}, 900:{items:3}}">
           <div v-for="salePoint in salePoints">
             <div class="px-2">
               <div class="card border-0 h-100">
                 <img :src="salePoint.img" alt="Sale Point" class="card-img rounded-0"/>
                 <div class="card-footer card-body py-4 rounded-0">
                   <p><i class="fas fa-store mr-2 mb-0 text-info"></i> Lorem ipsum dolor sit amet.</p>
                   <p><i class="fas fa-phone mr-2 mb-0 text-info"></i> 0-000-0000</p>
                   <a href="" class="btn btn-info btn-sm">Shop Online</a>
                 </div>
               </div>
             </div>
           </div>
          </carousel>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import carousel from 'vue-owl-carousel'

export default {
  name: "SalePoint",
  components: { carousel },
  data () {
    return {
      salePoints: [
        // {
        //   id: 1,
        //   img: '../../static/images/sale-1.jpg',
        //   store: 'Lorem ipsum dolor sit amet.',
        //   phone: '0-000-0000',
        //   online_link: ''
        // },
        {
          id: 2,
          img: '../../static/images/sale-2.jpg',
          store: 'Lorem ipsum dolor sit amet.',
          phone: '0-000-0000',
          online_link: ''
        },
        {
          id: 3,
          img: '../../static/images/sale-3.jpg',
          store: 'Lorem ipsum dolor sit amet.',
          phone: '0-000-0000',
          online_link: ''
        },
        {
          id: 4,
          img: '../../static/images/sale-4.jpg',
          store: 'Lorem ipsum dolor sit amet.',
          phone: '0-000-0000',
          online_link: ''
        },
        {
          id: 5,
          img: '../../static/images/sale-5.jpg',
          store: 'Lorem ipsum dolor sit amet.',
          phone: '0-000-0000',
          online_link: ''
        }

      ]
    }
  }
}
</script>

<style scoped>
  .card-footer
  {
    border-top: 3px solid #17a2b8;
  }

</style>
