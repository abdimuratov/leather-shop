<template>
  <div>
    <WideImageCard />
  </div>
</template>

<script>
import WideImageCard from '../components/WideImageCard.vue'

export default {
  components: {
    WideImageCard,
  }
}
</script>

<style lang="scss" scoped>
.home-container {
  height: 100%;
  margin: 0;
}

.background {
  background-image: url("../assets/images/background.png");
  height: 100%;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
