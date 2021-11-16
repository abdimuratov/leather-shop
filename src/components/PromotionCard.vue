<template>
  <div class="card-margin promotion">
    <div class="promotion-background"></div>
    <div style="z-index: -1" class="dark-background"></div>
    <img src="../assets/images/sticker.png" alt="" class="promotion-sticker" />

    <div class="promotion-info">
      <span class="text-primary title">Защита от воды</span>
      <div class="description">
        <span>Поход в горы или холодная погода? Не проблема!</span>
        <span
          >Закажите к зиме индивидуальный фасон, не уступающий в качестве другой
          обуви.</span
        >
      </div>
    </div>

    <div class="promotion-links">
      <button class="big-button">Мужские</button>

      <button class="big-button">Женские</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.promotion {
  position: relative;
  display: flex;
  flex-direction: column;
  height: 70vh;
  padding-bottom: 90px;

  &-background {
    position: absolute;
    z-index: -2;
    width: 100%;
    height: 100%;
    background: url("../assets/images/promotion.png") 100% 100% no-repeat;
    background-size: cover;
    background-position: center;
  }

  &-sticker {
    position: absolute;
    top: 16px;
    left: 16px;
    width: 10%;
    z-index: -1;
  }

  &-info {
    display: flex;
    flex-direction: column;
    margin-top: auto;
    margin-left: auto;
    margin-right: auto;
    padding: 75px 90px;
  }

  &-links {
    display: flex;
    flex-direction: row;
    justify-content: center;

    & button:not(:last-child) {
      margin-right: 76px;
    }
  }
}

.title {
  font-size: 96px;
}

.description {
  display: flex;
  flex-direction: column;
  font-size: 24px;
}

@media screen and (max-width: 1024px) {
  .promotion {
    padding-bottom: 50px;
    height: fit-content;
  }

  .title {
    font-size: 48px;
  }

  .description {
    font-size: 12px;
  }
}

@media screen and(max-width: 767px) {
  .promotion {
    &-info {
      padding: 50px 40px;
    }
    
    &-links {
      & button:not(:last-child) {
        margin-right: 10px;
      }
    }
  }

  .title {
    font-size: 32px;
  }

  .description {
    font-size: 12px;
  }
}

@media screen and(max-width: 424px) {
  .promotion {
    &-links {
      flex-direction: column;
      align-items: center;

      & button:not(:last-child) {
        margin-right: 0;
        margin-bottom: 10px;
      }
    }
  }
}
</style>
