<template>
  <div class="home">
    <WelcomeComponent/>
    <aboutMeComponent></aboutMeComponent>
  </div>
</template>

<script>
// @ is an alias to /src
import WelcomeComponent from '@/components/WelcomeComponent.vue'
import AboutMeComponent from '@/components/AboutMeComponent'

export default {
  name: 'Home',
  components: {
    WelcomeComponent,
    AboutMeComponent
  }
}
</script>

// https://jacekjeznach.com/