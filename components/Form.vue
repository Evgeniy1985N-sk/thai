<script setup lang="ts">

</script>

<template>
  <section class="form-section">
    <div class="container">
      <div class="form-section__inner">
        <div class="form-section__title h1">
          Выбрали экскурсию?
        </div>
        <p class="form-section__text">
          Свяжитесь с нами и мы ответим на все вопросы и поможем организовать ваш отдых
        </p>
        <form class="form-section__form">
          <input class="form-input" type="text" placeholder="Ваше имя">
          <input class="form-input" type="tel" placeholder="Контактный телефон">
          <button class="form-section__button button button-secondary">
            Отправить
          </button>
          <label class="check">
            <input class="check__input" type="checkbox">
            <i class="check__square"></i>
            <span class="check__text">
              Я согласен с <a href="#">политикой конфиденциальности</a>
            </span>
          </label>
        </form>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
  @use '@/assets/components/Form.scss';
</style>