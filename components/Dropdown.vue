<template>
  <div class="dropdown" :class="{ dropdown_active: isOpen }">
    <button 
      @click="toggleDropdown"
      class="dropdown__button" 
      >
      {{ selectedOption || placeholderText }}
    </button>
    <div v-if="isOpen" class="dropdown__content">
      <div
        v-for="option in options"
        :key="option"
        @click="selectOption(option)"
        class="dropdown__item"
      >
        {{ option }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    options: {
      type: Array,
      required: true
    },
    placeholderText: {
      type: String,
      default: 'Выберите опцию'
    }
  },
  data() {
    return {
      isOpen: false,
      selectedOption: null
    };
  },
  methods: {
    toggleDropdown() {
      this.isOpen = !this.isOpen;
    },
    selectOption(option) {
      this.selectedOption = option;
      this.isOpen = false;
    }
  }
};
</script>

<style lang="scss" scoped>

  .dropdown {
    position: relative;

    &__button {
      position: relative;
      width: 100%;
      height: 40px;
      padding: 8px 20px;
      text-align: left;
      font-weight: 500;
      font-size: 14px;
      line-height: 140%;
      text-transform: uppercase;
      color: rgba(13, 6, 38, 0.8);

      border: 1px solid #ddc61c;
      border-radius: 100px;
      background: transparent;
      &:after {
        content: '⏷';
        position: absolute;
        top: 50%;
        right: 20px;
        transform: translateY(-50%);
        font-size: 20px;
      }
    }
    &__content {
      display: block;
      position: absolute;
      background-color: #f9f9f9;
      min-width: 100%;
      box-shadow: 0px 8px 16px 0px rgba(0,0,0,0.2);
      z-index: 1;
    }
    &__item {
      padding: 12px 16px;
      text-decoration: none;
      display: block;
      cursor: pointer;
      transition: .2s;
      &:hover {
        background-color: #f1f1f1;
      }
    }

    &_active {
      .dropdown__button:after {
        transform: translateY(-50%) scale(-1,-1);
      }
      .dropdown__content {
        z-index: 2;
      }
    }
  }

</style>