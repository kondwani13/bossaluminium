<script>
import { ref, watch, toRefs } from 'vue'
import { Navigation, Pagination, A11y, Lazy, Thumbs } from 'swiper'
import { Swiper, SwiperSlide } from 'swiper/vue'

export default {
  components: {
    Swiper, 
    SwiperSlide
  },
  props: {
    currentSlide: Number,
    thumbs: Object
  },

   data() {
  return{ 
    
      };
   },

  

  setup(props) {
    const swiperRef = ref(null)

    const { currentSlide } = toRefs(props)

    watch(currentSlide, () => {
      if(swiperRef.value !== null) {
        swiperRef.value.slideTo(props.currentSlide)
      }
    })

    const onSwiper = (swiper) => {
      swiperRef.value = swiper
    }

    return {
      swiperRef,
      onSwiper,
      Navigation, 
      Pagination, 
      A11y, 
      Lazy, 
      Thumbs,
      images: [
     {
    src:'https://i.postimg.cc/HnS57PPt/c1.jpg',
    alt:'j1',
    id:0
    },
    {
    src:'https://i.postimg.cc/VL6XcmdZ/c2.jpg',
    alt:'c1',
    id:1
    },
    {
    src:'https://i.postimg.cc/qBQ2YzMC/c5.jpg',
    alt:'w6',
    id:2
    },
    {
    src:'https://i.postimg.cc/JnLbwXkj/j2.jpg',
    alt:'w4',
    id:3
    },
    {
    src:'https://i.postimg.cc/HnWXnC3x/j3.jpg',
    alt:'w3',
    id:4
    },
    {
    src:'https://i.postimg.cc/3RF23wXV/p1.jpg',
    alt:'w2',
    id:5
    },
    {
    src:'https://i.postimg.cc/hGFmxmMN/p2.jpg',
    alt:'p9',
    id:6
    },
    {
    src:'https://i.postimg.cc/qv6nzwc8/p4.jpg',
    alt:'p7',
    id:7
    },
    {
    src:'https://i.postimg.cc/8P0Mp9vp/p6.jpg',
    alt:'p6',
    id:8
    },
    {
    src:'https://i.postimg.cc/bvQtRvBr/p7.jpg',
    alt:'p9',
    id:9
    },
    {
    src:'https://i.postimg.cc/MT5fhFx8/p9.jpg',
    alt:'p5',
    id:10
    },
    {
    src:'https://i.postimg.cc/pTRnctwZ/w1.jpg',
    alt:'p1',
    id:11
    },
    {
    src:'https://i.postimg.cc/zvfH5FXH/w2.jpg',
    alt:'p5',
    id:12
    },
     {
    src:'https://i.postimg.cc/L50YsgnC/w3.jpg',
    alt:'p1',
    id:13
    },
     {
    src:'https://i.postimg.cc/8kyr49tR/w4.jpg',
    alt:'j3',
    id:14
    },
     {
    src:'https://i.postimg.cc/J4vHVJwt/w5.jpg',
    alt:'j2',
    id:15
    },
      ]
      
    }
  }
}
</script>

<template>
  <Swiper @swiper="onSwiper" :slides-per-view="1" :space-between="50" :modules="[Navigation, Pagination, A11y, Lazy, Thumbs]" navigation :pagination="{ clickable: true, dynamicBullets: true }" grab-cursor :preload-images="false" lazy :thumbs="{ swiper: thumbs }">
    <SwiperSlide v-for="(images, id) in images" :key="id" class="customSlide">
      <img :data-src="images.src" class="swiper-lazy" style="width: 640px; max-width: 100%" />
      <div class="swiper-lazy-preloader"></div>
    </SwiperSlide>
  </Swiper>
</template>

<style scoped>
.customSlide {
  display: grid;
  place-items: center;
  height: 100vh;
}
</style>