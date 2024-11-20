<style lang="scss">
</style>

<template>

  <Intro />

  <About />

  <Excursion />

  <Faq />

  <Reviews />

  <Form />
  
</template>


<style lang="scss" scoped>
  .tag-box {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    &__name {
        padding: 4px 12px;
        font-family: var(--font-family);
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
      font-size: 10px;
    }
  }
}
</style>