<template>
  <div class="home">
    <WelcomeComponent/>
    <MyPortfolioComponent></MyPortfolioComponent>
    <AboutMe></AboutMe>
  </div>
</template>

<script>
// @ is an alias to /src
import WelcomeComponent from '@/components/WelcomeComponent.vue'
import MyPortfolioComponent from '@/components/MyPortfolioComponent'
import AboutMe from '@/components/AboutMe.vue'

export default {
  name: 'Home',
  components: {
    WelcomeComponent,
    MyPortfolioComponent,
    AboutMe
  }
}
</script>
