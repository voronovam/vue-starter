<template>
  <div class="homePage">
    <Header />

    <div class="container">
      <div class="benefitsList">
        <h2 class="benefitsList__headline">Benefits headline</h2>
        <div class="benefitsList__body">
          <BenefitCard v-for="benefit in benefits" :key="benefit.id" :benefit="benefit" />
        </div>
      </div>
      <Slider />
    </div>
    <Price />
    <Footer />

  </div>
</template>

<script>
import Footer from "@/components/Footer";
import Header from "@/components/Header";
import BenefitCard from "@/components/BenefitCard";
import Slider from "@/components/Slider";
import Price from "@/components/Price";
export default {
  name: 'Home',
  data () {
    return {
      benefits: [
        {
          id: 1,
          icon: 'path_to_icon_1',
          title: 'Headline 1',
          text: 'Text 1',
        },
        {
          id: 2,
          icon: 'path_to_icon_2',
          title: 'Headline 2',
          text: 'Text 2',
        },
        {
          id: 3,
          icon: 'path_to_icon_3',
          title: 'Headline 3',
          text: 'Text 3',
        },
        {
          id: 4,
          icon: 'path_to_icon_4',
          title: 'Headline 4',
          text: 'Text 4',
        }
      ]
    }
  },
  components: {
    Price,
    Slider,
    BenefitCard,
    Header,
    Footer
  }
}
</script>

<style scoped lang="sass">
.homePage
  display: flex
  flex-direction: column
  height: 100vh

.benefitsList
  padding: 80px 0
  &__headline
    text-align: center
    margin-bottom: 50px
  &__body
    display: flex
    justify-content: space-between
    gap: 10px
</style>