<template>
  <div id="app">
      <!-- <LoadingScreen v-show="isLoading" ></LoadingScreen> -->
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
    </div> -->
    <!-- <MyPortfolioComponent v-show="!false" @openProjectModal='openModal' ></MyPortfolioComponent> -->
    <!-- <ProjectModal v-show="isProjectModalVisible" >
    </ProjectModal> -->
    <!-- @close="closeProjectModal" -->
    <router-view/>


  </div>
</template>


<script>
// import ProjectModal from "@/components/MyPortfolio/ProjectModal";
// import MyPortfolioComponent from '@/components/MyPortfolioComponent'
// import LoadingScreen from '@/components/LoadingScreen.vue'
export default {
    data(){
        return{
            isLoading: true,
            isProjectModalVisible: false,
        }
    },
    components: {
        // LoadingScreen,
        // ProjectModal,
        // MyPortfolioComponent,
    },
    mounted() {
    setTimeout(() => {
      this.isLoading = false
    }, 2000)
  },
//   methods:{
//       openModal(){
//           console.log('openModal');
//           this.isProjectModalVisible = true;
//       }
//   }
}
</script>

<style lang="less">

@main-color: #1e1e1e;

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>


<style src="./assets/styles/css/style.css"/>
