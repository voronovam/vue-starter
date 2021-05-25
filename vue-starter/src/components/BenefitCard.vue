<template>
  <div class="benefitCard">
    <div>{{benefit.icon}}</div>
    <h3>{{benefit.title}}</h3>
    <p>{{benefit.text}}</p>
  </div>
</template>

<script>
export default {
  name: "BenefitCard",
  props: {
    benefit: {
      type: Object,
      default: () => ({})
    }
  }
}
</script>

<style scoped lang="sass">
.benefitCard
  box-shadow: $box-shadow
  padding: 20px
  border-radius: $border-radius
</style>