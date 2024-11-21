
<template>
  <section class="excursion">
    <div class="container">
      <h1 class="excursion__title h1">
        каталог Экскурсий
      </h1>

      <div class="excursion__dropdowns">
        <Dropdown 
          :options="['Опция 1', 'Опция 2', 'Опция 3']" 
          placeholderText="Страна"
        />
        <Dropdown 
          :options="['Опция 1', 'Опция 2', 'Опция 3']" 
          placeholderText="Город" 
        />
        <Dropdown 
          :options="['Опция 1', 'Опция 2', 'Опция 3']" 
          placeholderText="Тип"
        />
        <Dropdown 
          :options="['Опция 1', 'Опция 2', 'Опция 3']" 
          placeholderText="длительность"
        />
        <Dropdown 
          :options="['Опция 1', 'Опция 2', 'Опция 3']" 
          placeholderText="Цена"
        />
      </div>

      <div class="excursion__items">

        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-1.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-2.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-3.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-4.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-5.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-6.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-7.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-8.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-9.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-10.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-11.jpg" alt="photo">
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
        <div class="excursion-item">
          <img class="excursion-item__img" src="/assets/images/catalog-image-12.jpg" alt="photo">
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
     
      </div>

    </div>
  </section>
</template>



<style lang="scss" scoped>
  @use '@/assets/components/Excursion2.scss';
</style>

<script lang="ts">
  import Dropdown from './Dropdown.vue';

  export default {
    components: {
      Dropdown
    }
  };
</script>