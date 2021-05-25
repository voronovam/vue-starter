<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__body">
        <LogoMain modifier="footer" />
        <Socials />
      </div>
    </div>
  </footer>
</template>

<script>
import LogoMain from "./LogoMain";
import Socials from "./Socials";
export default {
  name: "Footer",
  components: {Socials, LogoMain}
}
</script>

<style scoped lang="sass">
.footer
  background: linear-gradient(0deg, #043E44, #043E44), #CBE07D
  color: white
  padding: 50px 0
  margin-top: auto
  &__body
    display: flex
    justify-content: space-between
</style>