<template>
  <div class="home">
    <WelcomeComponent/>
    <MyPortfolioComponent></MyPortfolioComponent>
  </div>
</template>

<script>
// @ is an alias to /src
import WelcomeComponent from '@/components/WelcomeComponent.vue'
import MyPortfolioComponent from '@/components/MyPortfolioComponent'

export default {
  name: 'Home',
  components: {
    WelcomeComponent,
    MyPortfolioComponent
  }
}
</script>
