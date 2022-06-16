<template>
  <section class="carousel">
    <div class="carousel__item">
      <div class="first-item">
        <img src="../../assets/img/client-logos-3.png" alt="" />
      </div>
      <div>
        <img src="../../assets/img/client-logos-1.png" alt="" />
      </div>
      <div>
        <img src="../../assets/img/client-logos-4.png" alt="" />
      </div>
      <div>
        <img src="../../assets/img/client-logos-3.png" alt="" />
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "CarouselSection",
};
</script>

<style lang="scss" scoped>
.carousel {
  height: 250px;
  background: rgb(83, 188, 183);
  background: linear-gradient(
    90deg,
    rgba(83, 188, 183, 1) 0%,
    rgba(84, 130, 195, 1) 100%
  );

  &__item {
    height: 250px;
    text-align: center;
    justify-content: center;
    display: flex;
    width: 50%;
    align-items: center;
    margin: auto;

    img{
        width: 100%;
        height: auto;
    }

   
  }
}
</style>