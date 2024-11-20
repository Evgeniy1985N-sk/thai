<style lang="scss">
</style>


<template>

  <Intro />

  <About2 />

  <Accordion />

  <Gallery />

  <Reviews />

  <Slider />

  <Form />
  
</template>





<script lang="ts">
  import { Swiper, SwiperSlide } from 'swiper/vue';
  
  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      // Объявляем переменную swiperInstance с правильным типом
      const swiperInstance = ref<any>(null); // Используйте any, чтобы избежать проблем с типами
      // Функция для получения экземпляра Swiper
      const onSwiper = (swiper: any) => {
        swiperInstance.value = swiper;
      };
      const slideNext = () => {
      if (swiperInstance.value) {
        swiperInstance.value.slideNext(); // Вызываем метод slideNext
      }
    };
    const slidePrev = () => {
      if (swiperInstance.value) {
        swiperInstance.value.slidePrev(); // Вызываем метод slidePrev
      }
    };
      return {
        onSwiper,
        slideNext,
        slidePrev,
      };
    }
    
  };

</script>



<style lang="scss" scoped>
  .tag-box {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 4px;
    &__name {
        padding: 4px 12px;
        font-weight: 500;
        font-size: 8px;
        line-height: 140%;
        text-transform: uppercase;
        border: 1px solid rgba(221, 198, 28, 0.3);
        border-radius: 100px;
    }

    @media (min-width: breakpoints.$md) {
      &__name {
        padding: 6px 20px;
        font-size: 16px;
      }
    }
  }
</style>