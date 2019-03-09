<template>
  <div class="container">
    <div class="wrapper">
      <swiper :options="swiperOptions">
        <!-- slides -->
        <swiper-slide>
          <img class="gallary-img"
               src="http://img1.qunarzz.com/sight/p0/1509/d9/d94cb1d069d8e5dc.img.jpg_r_800x800_412d4350.jpg"/>
        </swiper-slide>
        <swiper-slide>
          <img class="gallary-img"
               src="http://img1.qunarzz.com/sight/p0/1509/be/be123bf4661627a8.img.jpg_r_800x800_0c9c5465.jpg"/>
        </swiper-slide>

        <!-- Optional controls -->
        <div class="swiper-pagination"  slot="pagination"></div>
      </swiper>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CommonGallary',
  data () {
    return {
      swiperOptions: {
        pagination: '.swiper-pagination',
        paginationType: 'fraction'
      }
    }
  }
}
</script>

<style lang="stylus" scoped>
  .container >>> .swiper-container
    overflow : inherit
  .container
    display :flex
    flex-direction : column
    justify-content : center
    position: fixed
    left : 0
    right : 0
    top:0
    bottom : 0
    background :#000
    z-index : 99
    .wrapper
      /*overflow : hidden*/
      width : 100%
      height : 0
      padding-bottom : 70%
      .gallary-img
        width : 100%
      .swiper-pagination
        color : #fff
        bottom : -1rem
</style>
