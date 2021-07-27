<template>
  <div>
    <div class="w-full h-auto lg:h-screen bg-color">
      <section
        id="section-work"
        class="py-5 lg:py-20 px-5 lg:px-20 flex flex-col lg:flex-row w-full lg:h-96"
      >
        <div id="text-zone" class=" w-full lg:w-1/2 h-auto flex flex-col">

          <PortfolioHeading></PortfolioHeading>
        <PortfolioDescription
            :portfolioDescription="portfolioDescription"
        ></PortfolioDescription>

        </div>

        <div
          id="text-zone"
          class="w-1/2 h-auto flex flex-col"
        ></div>

        <div class="work-big w-auto h-auto absolute">
          <h1 class="work-txt">Work</h1>
        </div>
      </section>
      
      <div class=" w-full h-auto flex m-auto border-2  z-10">

      <section class="px-0 mx-auto  max-w-10xl sm:px-0 lg:px-8 lg:py-4">
      <ul role="list" class="grid grid-cols-2 sm:grid-cols-2 md:grid-cols-4  lg:grid-cols-4">
      
      <Project
        :imageName="fitnessAppImage"
      ></Project>
      <Project
       :imageName="fitnessAppImage">

      </Project>
      <!-- <Projects></Projects>

     <Projects></Projects>
    <Projects></Projects>
    <Projects></Projects> -->
      </ul>
      </section>
      
      
      </div>

      

    

    </div>

    <!-- <div class="flex flex-col w-auto pl-4 border-2 border-white">
        <div class="w-auto h-auto flex flex-center pl-2 lg:ml-20 border-2 border-red-600">
          <h1 class="text-white text-5xl">My Portfolio</h1>
        </div>
        <div class="w-auto h-auto flex flex-center pl-2 lg:ml-20 border-2 border-blue-600">
          <p class="text-white h-auto  text-2xl">lorem10</p>
        </div>
      </div> -->


      
  </div>
</template>

<script>
import PortfolioHeading from "@/components/MyPortfolio/PortfolioHeading.vue";
import PortfolioDescription from "@/components/MyPortfolio/MyPortfolioDescription.vue";
import Project from "@/components/MyPortfolio/Project.vue"
export default {
  data() {
    return {
      fitnessAppImage: "fitnessApp.png",
      portfolioDescription: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean pretium mi sed sapien faucibus varius. Sed luctus justo ut mauris facilisis, a pulvinar orci blandit. Integer viverra in purus a faucibus. Proin ut rutrum massa, vitae interdum tortor.",
    };
  },
  components: {
    PortfolioHeading,
    PortfolioDescription,
    Project,
  },
};
</script>

<style lang="less">
.work-big {
  left: 60vh;
  margin-top: 6rem;
  z-index: 1;
  .work-txt {
    color: rgba(255, 255, 255, 0.05);
    font-size: 280px;
    font-weight: 600;
    letter-spacing: -15px;
  }
}



@media only screen and (max-width: 600px) {


.work-big {
  left: 18vh;
  margin-top: 2rem;
  z-index: 1;
  .work-txt {
    color: rgba(255, 255, 255, 0.05);
    font-size: 100px;
    font-weight: 600;
    letter-spacing: -8px;
    opacity: 0.5;
  }
}

}

</style>
