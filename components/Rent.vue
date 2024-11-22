
<template>
  <section class="rent">
    <div class="container">
      <h1 class="rent__title h1">
        Аренда авто
      </h1>
      <div class="rent__items">
        <div class="rent__item">
          <div class="rent__gallery">
            <swiper
              :class="{ 'rent__slider': true }"
              :slides-per-view="1"
              :space-between="0"
              @swiper="onSwiper"
            >
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-1.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-2.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-3.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-4.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-5.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-6.jpg" alt="">
              </swiper-slide>
            </swiper>
            <div class="rent__wrapper-img">
                <img class="rent__img" src="/assets/images/rent-img-2.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
                <img class="rent__img" src="/assets/images/rent-img-3.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
                <img class="rent__img" src="/assets/images/rent-img-4.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
                <img class="rent__img" src="/assets/images/rent-img-5.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
                <img class="rent__img" src="/assets/images/rent-img-6.jpg" alt="">
            </div>
          </div>
          <div class="rent__content">
            <div class="rent__content-title">
              Седан / хетчбек
            </div>
            <div class="rent__tag-box tag-box">
              <span class="tag-box__name">
                Дизель
              </span>
              <span class="tag-box__name">
                Автомат
              </span>
              <span class="tag-box__name">
                Полный привод
              </span>
              <span class="tag-box__name">
                кондиционер
              </span>
            </div>
            <div class="rent-table">
              <div class="rent-table__head">
                  <div>
                    <div class="rent-table__head-title">
                      Сутки
                    </div>
                    <p class="rent-table__head-text">
                      1200 В / день
                    </p>
                  </div>
                  <div>
                    <div class="rent-table__head-title">
                      Неделя
                    </div>
                    <p class="rent-table__head-text">
                      1000 В / день
                    </p>
                  </div>
                  <div>
                    <div class="rent-table__head-title">
                      Месяц
                    </div>
                    <p class="rent-table__head-text">
                      600 В / день
                    </p>
                  </div>
              </div>
              <div class="rent-table__body">
                <div class="rent-table__body-head">
                  <div class="rent-table__body-title">
                    Марка
                  </div>
                  <div class="rent-table__body-title">
                    Год выпуска
                  </div>
                  <div class="rent-table__body-title">
                    Кол-во мест
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="rent__item">
          <div class="rent__gallery">
            <swiper
              :class="{ 'rent__slider': true }"
              :slides-per-view="1"
              :space-between="0"
              @swiper="onSwiper"
            >
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-7.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-8.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-9.jpg" alt="">
              </swiper-slide>
            </swiper>
            <div class="rent__wrapper-img">
                <img class="rent__img" src="/assets/images/rent-img-8.jpg" alt="">
              </div>
              <div class="rent__wrapper-img">
                <img class="rent__img" src="/assets/images/rent-img-9.jpg" alt="">
              </div>
          </div>
          <div class="rent__content">
            <div class="rent__content-title">
              кроссовер
            </div>
            <div class="rent__tag-box tag-box">
              <span class="tag-box__name">
                Дизель
              </span>
              <span class="tag-box__name">
                Автомат
              </span>
              <span class="tag-box__name">
                Полный привод
              </span>
              <span class="tag-box__name">
                кондиционер
              </span>
            </div>
            <div class="rent-table">
              <div class="rent-table__head">
                  <div>
                    <div class="rent-table__head-title">
                      Сутки
                    </div>
                    <p class="rent-table__head-text">
                      1200 В / день
                    </p>
                  </div>
                  <div>
                    <div class="rent-table__head-title">
                      Неделя
                    </div>
                    <p class="rent-table__head-text">
                      1000 В / день
                    </p>
                  </div>
                  <div>
                    <div class="rent-table__head-title">
                      Месяц
                    </div>
                    <p class="rent-table__head-text">
                      600 В / день
                    </p>
                  </div>
              </div>
              <div class="rent-table__body">
                <div class="rent-table__body-head">
                  <div class="rent-table__body-title">
                    Марка
                  </div>
                  <div class="rent-table__body-title">
                    Год выпуска
                  </div>
                  <div class="rent-table__body-title">
                    Кол-во мест
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="rent__item">
          <div class="rent__gallery">
            <swiper
              :class="{ 'rent__slider': true }"
              :slides-per-view="1"
              :space-between="0"
              @swiper="onSwiper"
            >
              <swiper-slide>
                <img class="rent__slider-img" src="/assets/images/rent-img-10.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-11.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-12.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-13.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-14.jpg" alt="">
              </swiper-slide>
              <swiper-slide>
                  <img class="rent__slider-img" src="/assets/images/rent-img-15.jpg" alt="">
              </swiper-slide>
            </swiper>
            <div class="rent__wrapper-img">
              <img class="rent__img" src="/assets/images/rent-img-11.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
              <img class="rent__img" src="/assets/images/rent-img-12.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
              <img class="rent__img" src="/assets/images/rent-img-13.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
              <img class="rent__img" src="/assets/images/rent-img-14.jpg" alt="">
            </div>
            <div class="rent__wrapper-img">
              <img class="rent__img" src="/assets/images/rent-img-15.jpg" alt="">
            </div>
          </div>
          <div class="rent__content">
            <div class="rent__content-title">
              Седан / хетчбек
            </div>
            <div class="rent__tag-box tag-box">
              <span class="tag-box__name">
                Дизель
              </span>
              <span class="tag-box__name">
                Автомат
              </span>
              <span class="tag-box__name">
                Полный привод
              </span>
              <span class="tag-box__name">
                кондиционер
              </span>
            </div>
            <div class="rent-table">
              <div class="rent-table__head">
                  <div>
                    <div class="rent-table__head-title">
                      Сутки
                    </div>
                    <p class="rent-table__head-text">
                      1200 В / день
                    </p>
                  </div>
                  <div>
                    <div class="rent-table__head-title">
                      Неделя
                    </div>
                    <p class="rent-table__head-text">
                      1000 В / день
                    </p>
                  </div>
                  <div>
                    <div class="rent-table__head-title">
                      Месяц
                    </div>
                    <p class="rent-table__head-text">
                      600 В / день
                    </p>
                  </div>
              </div>
              <div class="rent-table__body">
                <div class="rent-table__body-head">
                  <div class="rent-table__body-title">
                    Марка
                  </div>
                  <div class="rent-table__body-title">
                    Год выпуска
                  </div>
                  <div class="rent-table__body-title">
                    Кол-во мест
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
                <div class="rent-table__body-row">
                  <div class="rent-table__body-text">
                    Toyota Fortuner
                  </div>
                  <div class="rent-table__body-text">
                    2016
                  </div>
                  <div class="rent-table__body-text">
                    4
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>



<style lang="scss" scoped>
  @use '@/assets/components/Rent.scss';
</style>

<script lang="ts">
</script>