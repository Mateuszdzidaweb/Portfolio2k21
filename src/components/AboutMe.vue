<template>
  <div>
    <div class="w-full h-auto lg:h-screen bg-color border-2">
      <section
        id="section-AboutMe"
        class="py-5 lg:py-20 px-5 lg:px-20 flex flex-col lg:flex-row w-full lg:h-auto border-2"
      >
        <div id="text-zone" class="w-full lg:w-1/2 h-auto flex flex-col ">
            <PersonalPhoto></PersonalPhoto>
        </div>

        <div id="text-zone" class="w-1/2 h-auto flex flex-col border-2"></div>

        <div class="work-big w-auto h-auto absolute">
          <h1 class="work-txt">About</h1>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
import PersonalPhoto from '@/components/About/PersonalPhoto'
export default {
    data(){
        return{

        }
    },
    components:{
        PersonalPhoto,
    }
}
</script>

<style lang="less">
    
    .image-overlay{
        // clip-path: polygon(25% 0,75% 0,90% 50%,75% 100%,25% 100%,30px 50%);
            // clip-path: ellipse(220px 255px at 10% 20%);
            clip-path: circle(45%);
            // border: 2px solid #00fdd7;
             shape-outside: border-box;
            background: rgba(0, 0, 0, 0.123);
    }
</style>
