<template>
  <div class="card-margin promotion">
    <div class="promotion-background"></div>
    <div style="z-index: -1;" class="dark-background"></div>
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
  padding: 0 0 90px 0;

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
  }

  &-info {
    display: flex;
    flex-direction: column;
    margin-top: auto;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 90px;
  }

&-links {
  display: flex;
  flex-direction: row;
  justify-content: center;

  &:not(:last-child):after {
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
</style>
