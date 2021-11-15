<template>
  <div class="card-container card-margin">
    <div class="item-group">
      <img src="../assets/images/wide1.png" alt="" />

      <div></div>
    </div>

    <div class="item-group">
      <img src="../assets/images/wide2.png" alt="" />

      <div></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card-container {
  display: flex;
  flex-direction: row;
  width: 100%;
  height: 100%;
  max-height: 600px;
}

.item-group {
  position: relative;

  &:first-child {
    margin-right: 10px;
  }

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  div {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.4);
    transition: all 1000ms ease-in-out;
    
    &:hover {
      background: none;
    }
  }
}
</style>
