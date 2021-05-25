<template>
  <header class="header">
    <div class="container">
      <LogoMain />
      <h1>Header</h1>
    </div>
  </header>
</template>

<script>
import LogoMain from "./LogoMain";
export default {
  name: "Header",
  components: {LogoMain}
}
</script>

<style scoped lang="sass">
.header
  padding: 50px 0
</style>