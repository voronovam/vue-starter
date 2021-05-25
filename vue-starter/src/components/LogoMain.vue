<template>
  <div
      class="logo"
      :class="modifier ? 'logo_' + modifier : ''"
  >Logo</div>
</template>

<script>
export default {
  name: "LogoMain",
  props: {
    modifier: {
      type: String,
      default: ''
    },
  }
}
</script>

<style scoped lang="sass">
.logo

  &_footer
    color: white
</style>