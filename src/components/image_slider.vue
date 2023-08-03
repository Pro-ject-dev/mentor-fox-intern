<template>
    <div class="carousel-container">
      <swiper :options="swiperOptions">
        <swiper-slide v-for="(image, index) in images" :key="index">
          <img :src="image" :alt="`Slide ${index + 1}`" />
          <div class="contents">
            <p class="c1">From Concept to creation, we bring</p>
            <p class="c1">your furniture dreams to life</p>
            <p class="c2">we specialize in creating unique, one-of-a-kind pieces tailored furniture</p>
            <div class="btn">
              <button>Customize Now</button>
            </div>
          </div>
        </swiper-slide>
      </swiper>
      <div v-if="paginationEnabled" class="swiper-pagination"></div>
    </div>
  </template>
  
  
  <script>
  import 'swiper/css';
  import 'swiper/css/bundle';
  import { Swiper, SwiperSlide } from 'vue-awesome-swiper';
  
  export default {
    name: 'img',
    components: {
      Swiper,
      SwiperSlide,
    },
    data() {
      return {
        images: [
          'https://firebasestorage.googleapis.com/v0/b/angry-bird-b4b71.appspot.com/o/WhatsApp%20Image%202023-08-01%20at%209.32.32%20PM.jpeg?alt=media&token=84d3b0e7-c803-455c-ade1-68ee696dc90d',
          'https://firebasestorage.googleapis.com/v0/b/mapview-aafa3.appspot.com/o/stylish-scandinavian-living-room-with-design-mint-sofa-furnitures-mock-up-poster-map-plants-eleg.jpg?alt=media&token=c44cae3c-e802-48ca-b674-58a723d3ae4d',
          'https://firebasestorage.googleapis.com/v0/b/mapview-aafa3.appspot.com/o/medium-shot-girl-holding-painting.jpg?alt=media&token=68e74836-255f-4c2a-bf4c-7a08ed08dfd1',
        ],
        swiperOptions: {
          loop: true,
          pagination: {
            el: '.swiper-pagination',
          },
          autoplay: {
            delay: 3000, 
          },
        },
      };
    },
    computed: {
      paginationEnabled() {
        return this.swiperOptions.pagination && this.swiperOptions.pagination.el;
      },
    },
  };
  </script>
  
  <style scoped>

.carousel-container {
  max-width: 100%;
  margin: 0 auto;
  position: relative;
}

img {
  width: 100%;
  max-height: 570px;
}

.contents {
  position: absolute;
  top: 32%;
  left: 18%;
  text-align: center;
  padding: 10px;
  border-radius: 5px;
  color: white;
}

.c1 {
  font-size: 2.45rem;
  font-weight: 700;
  font-family: 'Unbounded'
}

.c2 {
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
  padding-top: 8px;
}

button {
  height: 2.3rem;
  width: 10rem;
  padding-left: 5px;
  padding-right: 5px;
  background-color: rgb(255, 247, 0);
  font-size: 12px;
  font-family: 'Unbounded';
  font-weight: 800;
  border: 0px;
  display: block;
  margin: 0 auto;
}

.btn {
  padding: 20px;
}

@media screen and (max-width: 768px) {
  img {
    max-height: 400px;
  }

  .c1 {
    font-size: 28px;
  }

  .c2 {
    font-size: 14px;
  }

  button {
    height: 2.3rem;
    width: 20%;
    font-size: 10px;
  }
}

@media screen and (max-width: 480px) {
  img {
    max-height: 300px;
  }

  .c1 {
    font-size: 24px;
  }

  .c2 {
    font-size: 12px;
  }
  
  button {
    height: 2.3rem;
    width: 70%; 
    font-size: 12px; 
  }
}
  
</style>


  