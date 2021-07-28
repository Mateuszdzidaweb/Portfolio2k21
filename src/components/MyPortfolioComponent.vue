<template>
  <div>
    <div class="w-full h-auto lg:py-10 bg-color">
      <section
        id="section-work"
        class="py-5 px-5 lg:px-20 flex flex-col lg:flex-row w-full mx-auto lg:h-96"
      >
        <div
          id="text-zone"
          class="w-full xl:min-h-screen xl:justify-centerlg:w-1/2 xl:w-1/3 h-auto flex flex-col"
        >
          <PortfolioHeading></PortfolioHeading>

          <TextFade class="2xl:py-5" :textDescription="portfolioDescription"></TextFade>
        </div>

        <div
          id="text-zone"
          class="w-1/2 xl:min-h-screen xl:justify-center h-auto flex flex-col"
        ></div>

        <div class="work-big w-auto h-auto absolute">
          <h1 class="work-txt">Work</h1>
        </div>
      </section>

      <div class="w-full  h-auto flex justify-center z-10">
        <section class="px-0 mx-auto max-w-10xl sm:px-0 lg:px-8 lg:py-4 xl:py-10 md:w-full  ">
          <ul
            role="list"
            class=" grid grid-cols-2 mx-auto sm:grid-cols-2 md:flex md:flex-wrap  xl:w-2/3 "
          >
            <Project
              data-aos="zoom-in"
              data-aos-duration="1500"
              data-aos-anchor-placement="bottom-bottom"
              :imageName="fitnessAppImage"
            ></Project>
            <Project
              data-aos="zoom-in"
              data-aos-delay="300"
              data-aos-duration="1500"
              data-aos-anchor-placement="bottom-bottom"
              :imageName="fitnessAppImage"
            >
            </Project>
                        <Project
              data-aos="zoom-in"
              data-aos-delay="300"
              data-aos-duration="1500"
              data-aos-anchor-placement="bottom-bottom"
              :imageName="fitnessAppImage"
            >
            </Project>
                                    <Project
              data-aos="zoom-in"
              data-aos-delay="300"
              data-aos-duration="1500"
              data-aos-anchor-placement="bottom-bottom"
              :imageName="fitnessAppImage"
            >
            </Project>
                                    <Project
              data-aos="zoom-in"
              data-aos-delay="300"
              data-aos-duration="1500"
              data-aos-anchor-placement="bottom-bottom"
              :imageName="fitnessAppImage"
            >
            </Project>
                                                <Project
              data-aos="zoom-in"
              data-aos-delay="300"
              data-aos-duration="1500"
              data-aos-anchor-placement="bottom-bottom"
              :imageName="fitnessAppImage"
            >
            </Project>
            <!-- grid grid-cols-2 mx-auto sm:grid-cols-2 md:flex md:flex-wrap  border-2 -->
<!-- class="grid grid-cols-1 mx-auto sm:grid-cols-2 md:grid-cols-4 lg:grid-cols-4" -->
            <!-- <Projects></Projects>
md:flex md:flex-wrap md:justify-center
     <Projects></Projects>
    <Projects></Projects>
    <Projects></Projects> -->

          </ul>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import PortfolioHeading from "@/components/MyPortfolio/PortfolioHeading.vue";
import TextFade from "@/components/MyPortfolio/TextFade.vue";
import Project from "@/components/MyPortfolio/Project.vue";
export default {
  data() {
    return {
      fitnessAppImage: "fitnessApp.png",
      portfolioDescription:
        "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean pretium mi sed sapien faucibus varius. Sed luctus justo ut mauris facilisis, a pulvinar orci blandit. Integer viverra in purus a faucibus. Proin ut rutrum massa, vitae interdum tortor.",
    };
  },
  components: {
    PortfolioHeading,
    TextFade,
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

@media only screen and (max-width: 1280px) {
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
