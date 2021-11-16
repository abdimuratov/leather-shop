<template>
  <agile :options="myOptions" class="card-margin">
    <div v-for="(item, index) in items" :key="index" class="slide">
      <img :src="require(`@/assets/images/${item.imgName}`)" alt="Popular" />

      <div class="dark-background"></div>
    </div>
  </agile>
</template>

<script>
export default {
  data: () => ({
    myOptions: {
      navButtons: false,
      autoplay: true,
      autoplaySpeed: 5000,
      speed: 2500,
      fade: true,
      pauseOnHover: true,
      pauseOnDotsHover: true,
    },
    items: [
      { id: new Date().toString(), imgName: "carousel1.png", alt: "Popular" },
      { id: new Date().toString(), imgName: "carousel2.png", alt: "Popular" },
      { id: new Date().toString(), imgName: "carousel3.png", alt: "Popular" },
      { id: new Date().toString(), imgName: "carousel1.png", alt: "Popular" },
      { id: new Date().toString(), imgName: "carousel2.png", alt: "Popular" },
      { id: new Date().toString(), imgName: "carousel3.png", alt: "Popular" },
      { id: new Date().toString(), imgName: "carousel1.png", alt: "Popular" },
    ],
  }),
}
</script>

<style lang="scss" scoped>
.slide {
  position: relative;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
</style>
