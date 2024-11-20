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

<template>
  <section class="slider">
    <div class="container">

        <div class="page__title-row title-row">
          <div class="title-row__info">
            похожее
          </div>
          <div class="slider__wrapper-nav">
            <h2 class="h2">
              Другие экскурсии на&nbsp;пхукете
            </h2>
            <div class="slider__nav">
              <div class="slider-prev slider-button" @click="slidePrev">
                <svg width="16" height="13" viewBox="0 0 16 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd" clip-rule="evenodd" d="M2.58835 6.75749L6.86559 10.9429L5.81649 12.015L0.225031 6.54357C0.0808446 6.40248 
                  -0.000422749 6.20925 -0.00042274 6.00752C-0.000422732 5.80578 0.0808446 5.61256 0.225031 5.47147L5.81649 -4.45093e-07L6.86559 1.0721L2.58841 
                  5.25749L15.999 5.25749L15.999 6.75749L2.58835 6.75749Z" fill="" />
                </svg>
              </div>
              <div class="slider-next slider-button" @click="slideNext">
                <svg width="16" height="13" viewBox="0 0 16 13" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd" clip-rule="evenodd" d="M2.58835 6.75749L6.86559 10.9429L5.81649 12.015L0.225031 6.54357C0.0808446 6.40248 
                  -0.000422749 6.20925 -0.00042274 6.00752C-0.000422732 5.80578 0.0808446 5.61256 0.225031 5.47147L5.81649 -4.45093e-07L6.86559 1.0721L2.58841 
                  5.25749L15.999 5.25749L15.999 6.75749L2.58835 6.75749Z" fill="" />
                </svg>
              </div>
            </div>
          </div>
        </div>

        <swiper
          :class="{ 'slider__swiper': true }"
          :slides-per-view="2"
          :space-between="10"
          @swiper="onSwiper"
          :breakpoints= "{
            992:{ slidesPerView:3, spaceBetween:20 },
          }"
        >
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image-2.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image-3.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image-4.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
          <swiper-slide>
            <div class="excursion-item">
              <img class="excursion-item__img" src="/assets/images/excursion-image.jpg" alt="photo">
              <div class="excursion-item__content">
                <div class="tag-box">
                  <span class="tag-box__name">
                    Таиланд
                  </span>
                  <span class="tag-box__name">
                    Пхукет
                  </span>
                  <span class="tag-box__name">
                    Водная
                  </span>
                  <span class="tag-box__name">
                    2 дня
                  </span>
                </div>
                <div class="excursion-item__title">
                  Остров Пхи-Пхи на скоростном картере  
                </div>
                <div class="excursion-item__price">
                  3999 В
                </div>
              </div>
            </div>
          </swiper-slide>
        </swiper>

    </div>
  </section>
</template>

<style lang="scss" scoped>
  @use '@/assets/components/Slider.scss';
  @use '@/assets/components/Excursion.scss';
</style>