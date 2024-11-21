<template>
  <section class="reviews">
    <div class="container">
        <div class="reviews__title-row title-row">
          <div class="title-row__info">
            Отзывы
          </div>
          <h2 class="h2">
            1017 отзывов о&nbsp;компании
          </h2>
        </div>

        <div class="reviews__items">

          <div class="reviews__item">

            <div class="reviews__info">
              <div class="reviews__info-title">
                Оставьте свой отзыв
              </div>
              <div class="reviews__noname reviews-noname">
                <div class="reviews-noname__wrapper-img">
                  <img src="/assets/images/reviews-nophoto.png" width="43" height="43" alt="no photo">
                </div>
                <div class="reviews-noname__wrapper-text">
                  <p class="reviews-noname__text">
                    Ваше имя
                  </p>
                  <div class="reviews-noname__social reviews-social">
                    <div class="reviews-social__icons">
                      <a class="reviews-social__icon" href="#">
                        <img class="reviews-social__img" src="/assets/images/reviews-icon-1.svg" width="20" height="20" alt="social icon">
                      </a>
                      <a class="reviews-social__icon" href="#">
                        <img class="reviews-social__img" src="/assets/images/reviews-icon-2.svg" width="20" height="20" alt="social icon">
                      </a>
                      <a class="reviews-social__icon" href="#">
                        <img class="reviews-social__img" src="/assets/images/reviews-icon-3.svg" width="20" height="20" alt="social icon">
                      </a>
                    </div>
                    <p class="reviews-social__text">
                      Войди чрез соцсеть и мы заполним имя и аватар
                    </p>
                  </div>
                </div>
              </div>
              <div class="reviews__social-desk reviews-social">
                <p class="reviews-social__text">
                  Войди чрез соцсеть и мы заполним имя и аватар
                </p>
                <div class="reviews-social__icons">
                  <a class="reviews-social__icon" href="#">
                    <img class="reviews-social__img" src="/assets/images/reviews-icon-1.svg" width="20" height="20" alt="social icon">
                  </a>
                  <a class="reviews-social__icon" href="#">
                    <img class="reviews-social__img" src="/assets/images/reviews-icon-2.svg" width="20" height="20" alt="social icon">
                  </a>
                  <a class="reviews-social__icon" href="#">
                    <img class="reviews-social__img" src="/assets/images/reviews-icon-3.svg" width="20" height="20" alt="social icon">
                  </a>
                </div>
              </div>
            </div>

            <div class="reviews__content">
              <div class="reviews__content-title">
                Оставьте свой отзыв
              </div>
              <div class="reviews__content-stars reviews-stars">
                <div class="reviews-stars__item">
                  <img class="reviews-stars__img" src="/assets/images/reviews-star-1.svg" width="22" height="22" alt="star">
                </div>
                <div class="reviews-stars__item">
                  <img class="reviews-stars__img" src="/assets/images/reviews-star-1.svg" width="22" height="22" alt="star">
                </div>
                <div class="reviews-stars__item">
                  <img class="reviews-stars__img" src="/assets/images/reviews-star-1.svg" width="22" height="22" alt="star">
                </div>
                <div class="reviews-stars__item">
                  <img class="reviews-stars__img" src="/assets/images/reviews-star-1.svg" width="22" height="22" alt="star">
                </div>
                <div class="reviews-stars__item">
                  <img class="reviews-stars__img" src="/assets/images/reviews-star-1.svg" width="22" height="22" alt="star">
                </div>
              </div>
              <form class="reviews-form">
                <div class="reviews-form__wrapper-textarea">
                  <textarea class="reviews-form__textarea" placeholder="Напишите отзыв о компании здесь"></textarea>
                  <label class="reviews-file">
                    <input class="reviews-file__input" type="file">
                  </label>
                </div>
                <button class="reviews-form__button button button-primary" type="submit">
                    Отправить отзыв
                </button>
              </form>
            </div>

          </div>

          <div class="reviews__item">

            <div class="reviews__info">
              <div class="reviews-avatar">
                <img class="reviews-avatar__img" src="/assets/images/reviews-avatar-1.png" width="55" height="55" alt="no photo">
                <div class="reviews-avatar__wrapper-text">
                  <p class="reviews-avatar__text">
                    Максим
                  </p>
                  <span class="reviews-avatar__dsc">
                    2 экскурсии
                  </span>
                </div>
              </div>
            </div>

            <div class="reviews__content">

              <div class="reviews__wrapper-stars">
                <div class="reviews-stars">
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-3.svg" width="22" height="22" alt="star">
                  </div>
                </div>
                <span class="reviews__date">
                  21 августа 2024
                </span>
              </div>

              <div class="reviews__comment reviews-comment">
                <div class="reviews-comment__wrapper-text" :class="{ active: isActive }">
                  <div class="reviews-comment__text">
                    <p>
                      Трансфер приехал в назначенное время, подобрали несколько человек из отелей по пути и добрались до назначенного места. 
                      Там нас встретил Дмитрий, который позже сопровождал нас на всех станциях, снимал происходящее, рассказывал и объяснял, за что ему 
                      огромное спасибо! Слонов кормим, купаем, трем щетками - полный спа. На территории после мастер класс по приготовлению пары тайских блюд, 
                      которые потом благополучно съели, помимо них было еще что поесть, чай, кофе, вода. Рекомендую однозначно
                    </p>
                  </div>
                  <div class="reviews-comment__more" @click="setActive">
                    Читать полностью
                  </div>
                </div>
                <div class="reviews-comment__media">
                  <img src="/assets/images/reviews-image-1.jpg" width="100" height="100" alt="image">
                  <img src="/assets/images/reviews-image-2.jpg" width="100" height="100" alt="image">
                </div>
              </div>


            </div>

          </div>

          <div class="reviews__item">

            <div class="reviews__info">
              <div class="reviews-avatar">
                <img class="reviews-avatar__img" src="/assets/images/reviews-avatar-2.png" width="55" height="55" alt="no photo">
                <div class="reviews-avatar__wrapper-text">
                  <p class="reviews-avatar__text">
                    Артемий
                  </p>
                  <span class="reviews-avatar__dsc">
                    5 экскурсий
                  </span>
                </div>
              </div>
            </div>

            <div class="reviews__content">

              <div class="reviews__wrapper-stars">
                <div class="reviews-stars">
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-3.svg" width="22" height="22" alt="star">
                  </div>
                </div>
                <span class="reviews__date">
                  21 августа 2024
                </span>
              </div>

              <div class="reviews__comment reviews-comment">
                <div class="reviews-comment__wrapper-text" :class="{ active: isActive }">
                  <div class="reviews-comment__text">
                    <p>
                      Мы брали расширенную экскурсию, не пожалели. Организация отличная, без задержек. Слоников много, приготовили корм, кормили много, мыли, купали, плюс купание со слоном в водоеме. Времени для общения со слонами более чем достаточно, никто никуда не подгоняет. Из удобств, есть душ где ополоснуться, выдают сухие полотенца. Берите на смену сухую одежду. У нас входил обед, плюс мы сами готовили два тайских блюда, как всегда в Тае по максимуму. Нам все очень понравилось, после экскурсии мы выбрали вместо трансфера до отеля ближайший пляж еще там потусили пару часов, встретили закат и поехали  домой на такси, день сложился полноценно, за рекомендацию пляжа отдельное спасибо. На месте нас встречал русскоговорящий гид Дмитрий ( отдельный респект), в беде вас не оставят все подскажут и помогут, сделали кучу фото. Вообщем рекомендую в копилочку эмоций.
                    </p>
                  </div>
                  <div class="reviews-comment__more" @click="setActive">
                    Читать полностью
                  </div>
                </div>
              </div>


            </div>

          </div>

          <div class="reviews__item">

            <div class="reviews__info">
              <div class="reviews-avatar">
                <img class="reviews-avatar__img" src="/assets/images/reviews-avatar-3.png" width="55" height="55" alt="no photo">
                <div class="reviews-avatar__wrapper-text">
                  <p class="reviews-avatar__text">
                    Людмила
                  </p>
                  <span class="reviews-avatar__dsc">
                    12 экскурсий
                  </span>
                </div>
              </div>
            </div>

            <div class="reviews__content">

              <div class="reviews__wrapper-stars">
                <div class="reviews-stars">
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-3.svg" width="22" height="22" alt="star">
                  </div>
                </div>
                <span class="reviews__date">
                  21 августа 2024
                </span>
              </div>

              <div class="reviews__comment reviews-comment">
                <div class="reviews-comment__wrapper-text" :class="{ active: isActive }">
                  <div class="reviews-comment__text">
                    <p>
                      Огромный восторг от экскурсии. Невероятное тепло от общения с этими удивительными созданиями, у деткй гамма эмоций от "что то я боюсь его" до "стой спокойно, моя бусинка, я тебя помою", очень экологично, нет ощущения "зоопарка" 
                    </p>
                    <p>
                      Дмитрий замечательно провёл экскурсию, очень внимательный, подробно всё объясняет, фотографировал, мы вообще не заморачивались и получали удовольствие, + бонус - можно перевести оплату на российскую карту, что в наше "смутное" время становится актуальным и удобным
                    </p>
                  </div>
                  <div class="reviews-comment__more" @click="setActive">
                    Читать полностью
                  </div>
                </div>
                <div class="reviews-comment__media">
                  <img src="/assets/images/reviews-image-3.jpg" width="100" height="100" alt="image">
                  <img src="/assets/images/reviews-image-4.jpg" width="100" height="100" alt="image">
                  <img src="/assets/images/reviews-image-5.jpg" width="100" height="100" alt="image">
                  <img src="/assets/images/reviews-image-6.jpg" width="100" height="100" alt="image">
                  <img src="/assets/images/reviews-image-7.jpg" width="100" height="100" alt="image">
                </div>
              </div>


            </div>

          </div>

          <div class="reviews__item">

            <div class="reviews__info">
              <div class="reviews-avatar">
                <img class="reviews-avatar__img" src="/assets/images/reviews-avatar-4.png" width="55" height="55" alt="no photo">
                <div class="reviews-avatar__wrapper-text">
                  <p class="reviews-avatar__text">
                    Александр
                  </p>
                  <span class="reviews-avatar__dsc">
                    2 экскурсии
                  </span>
                </div>
              </div>
            </div>

            <div class="reviews__content">

              <div class="reviews__wrapper-stars">
                <div class="reviews-stars">
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-3.svg" width="22" height="22" alt="star">
                  </div>
                </div>
                <span class="reviews__date">
                  21 августа 2024
                </span>
              </div>

              <div class="reviews__comment reviews-comment">
                <div class="reviews-comment__wrapper-text" :class="{ active: isActive }">
                  <div class="reviews-comment__text">
                    <p>
                      Отличный гид, эрудированный, говорит на чистом русском, поэтому подойдет для гостей, которые не говорят по-английски. Сделал массу хороших фотографий, на этой экскурсии самому это сделать зачастую сложно. Рекомендую.
                    </p>
                  </div>
                  <div class="reviews-comment__more" @click="setActive">
                    Читать полностью
                  </div>
                </div>
              </div>


            </div>

          </div>

          <div class="reviews__item">

            <div class="reviews__info">
              <div class="reviews-avatar">
                <img class="reviews-avatar__img" src="/assets/images/reviews-avatar-5.png" width="55" height="55" alt="no photo">
                <div class="reviews-avatar__wrapper-text">
                  <p class="reviews-avatar__text">
                    Люба
                  </p>
                  <span class="reviews-avatar__dsc">
                    2 экскурсии
                  </span>
                </div>
              </div>
            </div>

            <div class="reviews__content">

              <div class="reviews__wrapper-stars">
                <div class="reviews-stars">
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-2.svg" width="22" height="22" alt="star">
                  </div>
                  <div class="reviews-stars__item">
                    <img class="reviews-stars__img" src="/assets/images/reviews-star-3.svg" width="22" height="22" alt="star">
                  </div>
                </div>
                <span class="reviews__date">
                  21 августа 2024
                </span>
              </div>

              <div class="reviews__comment reviews-comment">
                <div class="reviews-comment__wrapper-text" :class="{ active: isActive }">
                  <div class="reviews-comment__text">
                    <p>
                      Трансфер приехал в назначенное время, подобрали несколько человек из отелей по пути и добрались до назначенного места. Там нас встретил Дмитрий, который позже сопровождал нас на всех станциях, снимал происходящее, рассказывал и объяснял, за что ему огромное спасибо! Слонов кормим, купаем, трем щетками - полный спа. На территории после мастер класс по приготовлению пары тайских блюд, которые потом благополучно съели, помимо них было еще что поесть, чай, кофе, вода. Рекомендую однозначно
                    </p>
                  </div>
                  <div class="reviews-comment__more" @click="setActive">
                    Читать полностью
                  </div>
                </div>
              </div>


            </div>

          </div>

        </div>

        <button class="reviews__button button button-primary">
          Смотреть все отзывы
        </button>

    </div>
  </section>
</template>


<script lang="ts">

  export default {
    data() {
      return {
        isActive: false,
      };
    },
    methods: {
      setActive() {
        this.isActive = !this.isActive;
      },
    },

  };

</script>


<style lang="scss" scoped>
  @use '@/assets/components/Reviews.scss';
</style>