<template>
  <div class="card-container card-margin">
    <div class="item-group">
      <img src="../assets/images/wide1.png" alt="" />

      <div class="dark-background"></div>
    </div>

    <div class="item-group">
      <img src="../assets/images/wide2.png" alt="" />

      <div class="dark-background"></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  max-height: 600px;
  gap: 10px;
}

.item-group {
  position: relative;

  img {
    width: 100%;
    height: 100%;
    max-height: 600px;
    object-fit: cover;
  }
}
</style>
