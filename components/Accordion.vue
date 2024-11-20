<script lang="ts">
  import data from '~/data/accordion-data.js';
  
  export default {
    data() {
      return {
        items: data,
        isCntOpen: [] as boolean[]
      };
    },
    methods: {
      toggleCnt(index:number) {
        // Проверяем, открыто ли текущее состояние — если нет, открываем его
        const currentState = this.isCntOpen[index] || false;

        // Создаем новый массив по состоянию аккордеонов
        this.isCntOpen = this.isCntOpen.map((_, idx) => idx === index ? !currentState : false);
      }
    },
    mounted() {
      // Инициализируем состояние аккордеонов - все закрыты
      this.isCntOpen = this.items.map(() => false);
    },

  };

</script>

<template>
  <section class="accordion">
    <div class="container">
      <div class="accordion__wrapper">
        <div class="accordion__title">
          Дополнительная информация
        </div>
        <div class="accordion__items">

          <div 
            v-for="(item, index) in items" 
            :key="item.id" 
            :class="['accordion-item', { 'accordion-item_active': isCntOpen[index] }]"
          >
            <div class="accordion-item__title" @click="toggleCnt(index)">
              {{ item.title }}
            </div>
            <div 
              v-show="isCntOpen[index]"
              class="accordion-cnt"
              v-html="item.content"
            ></div>
          </div>


          <!-- <div class="accordion-item">
            <p class="accordion-item__text">
              программа
            </p>
            <div class="accordion-cnt">
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  День 1
                </div>
                <div class="accordion-cnt__content">
                  <div class="accordion-shedule">
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Выезд из отеля
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Прибытие к причалу, знакомство с гидом, перерыв на чай, кофе
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Отправление с причала
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Посещение бухты Майя, где проходили съемки фильма «Пляж» с Леонардо ДиКаприо
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Плавание в Лагуне Пиле
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Осмотр Пещеры Викингов
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        ОтПлавание с масками. Созерцание разнообразных видов рыб
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Отдых на прекрасном острове Бамбу
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Прибытие на острова Пхи Пхи Дон. Обед в пляжном ресторане
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Заселение в отель на острове Пхи-Пхи Дон. Посещение улиц деревни Пхи-Пхи, где есть множество модных баров, ресторанов и магазинов, время для отдыха
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Ужин в отеле
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        До начала пляжных вечеринок, посещение бара и возможность увидеть невероятное огненное шоу от чемпионов Таиланда, 
                        а также насладиться коктейлем на пляже
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Посещение бара, где самые смелые гости смогут попытать свои навыки в Тайском Боксе
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Ночная жизнь острова. Вечеринки на пляже
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Завтрак в отеле
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Время для отдыха после вечеринки на пляже, отдых на пляже
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Потрясающая возможность посетить обзорную площадку откуда открывается изумительный вид на остров
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Выселение с отеля
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Обед на острове Пхи Пхи Дон
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Осмотр пляжа обезьян в заливе Йонг Касем
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Плавание с масками возле островa Пхи-Пхи Дон. Созерцание разнообразных видов рыб
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Прибытие к причалу, отправление в отель
                      </p>
                    </div>
                    <div class="accordion-shedule__row">
                      <span class="accordion-shedule__time">
                        06:50
                      </span>
                      <p class="accordion-shedule__text">
                        Отправление с причала
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <p class="accordion-item__text">
              В стоимость входит
            </p>
            <div class="accordion-cnt">
              <div class="accordion-cnt__title">
                В стоимость входит
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Еда
                </div>
                <div class="accordion-cnt__content">
                  <p class="accordion-cnt__text">
                    2 обеда, 1 ужин, 1 завтрак, прохладительные напитки и свежие фрукты на борту
                  </p>
                </div>
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  транспорт
                </div>
                <div class="accordion-cnt__content">
                  <p class="accordion-cnt__text">
                    Автобус и лодка
                  </p>
                </div>
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Размещение
                </div>
                <div class="accordion-cnt__content">
                  <p class="accordion-cnt__text">
                    3-х звездочный отель Andaman Beach Resort или аналогичный
                  </p>
                </div>
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Дополнительно
                </div>
                <div class="accordion-cnt__content">
                  <p class="accordion-cnt__text">
                    Маски и трубки, страховка, вход в нац. парки, англо и русскоговорящий гид, опытные капитан и экипаж, спасательные жилеты
                  </p>
                </div>
              </div>
            </div>
          </div>
          <div class="accordion-item">
            <p class="accordion-item__text">
              Что взять с собой
            </p>
            <div class="accordion-cnt">
              <div class="accordion-cnt__title">
                Что взять с собой
              </div>
              <p class="accordion-cnt__text">
                Комфортную одежду и обувь, солнцезащитный крем и очки, паспорт
              </p>
            </div>
          </div>
          <div class="accordion-item">
            <p class="accordion-item__text">
              Трансфер
            </p>
            <div class="accordion-cnt">
              <div class="accordion-cnt__title">
                Трансфер
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Патонг/Калим
                </div>
                <p class="accordion-cnt__price">
                  100 В
                </p>
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Карон/Тритранг
                </div>
                <p class="accordion-cnt__price">
                  160 В
                </p>
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Ката
                </div>
                <p class="accordion-cnt__price">
                  200 В
                </p>
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Камала
                </div>
                <p class="accordion-cnt__price">
                  300 В
                </p>
              </div>
              <div class="accordion-cnt__row">
                <div class="accordion-cnt__info">
                  Сурин/Лагуна
                </div>
                <p class="accordion-cnt__price">
                  400 В
                </p>
              </div>
            </div>
          </div> -->

        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss">
  @use '@/assets/components/Accordion.scss';
</style>