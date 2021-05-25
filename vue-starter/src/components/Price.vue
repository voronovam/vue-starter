<template>
  <div class="price">
    <div class="container">
      <div class="price__list">
        <div v-for="item in prices" :key="item.id" class="price__box">
          <div>{{item.title}}</div>
          <div>{{item.price}}</div>
          <div>{{item.text}}</div>
        </div>
      </div>
      <div class="price__btnWrap">
        <button class="price__btn">Button</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Price",
  data(){
    return {
      prices: [
        {
          id: 1,
          title: 'Title 1',
          price: '100 ₽',
          text: 'Text price'
        },
        {
          id: 2,
          title: 'Title 2',
          price: 'delivery',
          text: 'Text'
        }
      ]
    }
  }
}
</script>

<style scoped lang="sass">
.price
  background: white
  padding: 80px 0
  &__list
    display: flex
    justify-content: center
    gap: 20px
  &__box
    border: 1px solid $color-accent
    border-radius: $border-radius
    padding: 20px
    width: 250px
  &__btnWrap
    text-align: center
  &__btn
    border: none
    padding: 20px
    background: $color-accent
    color: white
    min-width: 200px
    margin-top: 30px
    border-radius: $border-radius

</style>