<script>
import { Thumbs } from 'swiper'
import { Swiper, SwiperSlide } from 'swiper/vue'

export default {
  components: {
    Swiper, 
    SwiperSlide
  },
  props: {
    currentSlide: Number
  },

   data() {
  return{ 
    
      };
   }, 

  

  emits: ['thumbs', 'update:currentSlide'],
  setup(props, { emit }) {
    const onSwiper = (swiper) => {
      emit('thumbs', swiper)
    }

    return {
      onSwiper,
      Thumbs,
      images: [
    {
    src:'https://i.ibb.co/G9Q1PSS/j1.jpg',
    alt:'j1',
    id:0
    },
    {
    src:'https://i.ibb.co/tMmwh2q/c1.jpg',
    alt:'c1',
    id:1
    },
    {
    src:'https://i.ibb.co/hHbV2SW/w6.jpg',
    alt:'w6',
    id:2
    },
    {
    src:'https://i.ibb.co/5kL0SZd/w4.jpg',
    alt:'w4',
    id:3
    },
    {
    src:'https://i.ibb.co/4m43dzh/w3.jpg',
    alt:'w3',
    id:4
    },
    {
    src:'https://i.ibb.co/p3S6TBv/w2.jpg',
    alt:'w2',
    id:5
    },
    {
    src:'https://i.ibb.co/p3xb6Qp/p9.jpg',
    alt:'p9',
    id:6
    },
    {
    src:'https://i.ibb.co/tDstT43/p7.jpg',
    alt:'p7',
    id:7
    },
    {
    src:'https://i.ibb.co/PcFqG0r/p6.jpg',
    alt:'p6',
    id:8
    },
    {
    src:'https://i.ibb.co/p3xb6Qp/p9.jpg',
    alt:'p9',
    id:9
    },
    {
    src:'https://i.ibb.co/g6FSHrs/p5.jpg',
    alt:'p5',
    id:10
    },
    {
    src:'https://i.ibb.co/26Y9nXw/p1.jpg',
    alt:'p1',
    id:11
    },
    {
    src:'https://i.ibb.co/g6FSHrs/p5.jpg',
    alt:'p5',
    id:12
    },
     {
    src:'https://i.ibb.co/26Y9nXw/p1.jpg',
    alt:'p1',
    id:13
    },
     {
    src:'https://i.ibb.co/L0FZG2Z/j3.jpg',
    alt:'j3',
    id:14
    },
     {
    src:'https://i.ibb.co/2KvbS4P/j2.jpg',
    alt:'j2',
    id:15
    },
      ]
     
      
      
    }
  }
}
</script>

<template>
  <Swiper @swiper="onSwiper" :slides-per-view="10" :space-between="50" :modules="[Thumbs]" watch-slides-progress>
    <SwiperSlide v-for="(images, imagesId) in images" :key="imagesId" @click.stop="$emit('update:currentSlide')">
      <img :src="images.src"  style="height: 100px" />
    </SwiperSlide>
  </Swiper>
</template>