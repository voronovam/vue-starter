<template>
  <div class="slider">
    <h2 class="slider__headline">Slider headline</h2>
    <div class="slider__slide">Slide content</div>
  </div>
</template>

<script>
export default {
  name: "Slider"
}
</script>

<style scoped lang="sass">
.slider
  padding: 80px 0
  &__headline
    text-align: center
    margin-bottom: 50px
  &__slide
    background: $color-accent
    border-radius: $border-radius
    height: 200px
    width: 200px
    color: white
</style>