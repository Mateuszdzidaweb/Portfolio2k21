<template>
  <div>
    <div class="w-full h-auto lg:h-screen  lg:py-10 xl:py-0 bg-color">
      <section
        id="section-Contact"
        class="py-5 xl:py-0 px-5 lg:px-0 flex flex-col lg:flex-row lg:w-full 2xl-w-4/5 lg:m-auto lg:h-auto"
      >
        <div
          id="text-zone"
          class="w-full 2xl:items-center xl:min-h-screen xl:justify-center lg:w-2/3 lg:ml-10 h-auto flex flex-col py-10 lg:py-0"
        >
             <!-- <div class="flex border w-2/3">
        
             </div> -->
          <ContactForm></ContactForm>
        </div>

        <div
          id="text-zone"
          class="w-full xl:min-h-screen xl:justify-center lg:mr-10 lg:w-2/3 xl:w-1/3 h-auto flex flex-col justify-center "
        >
        
        <Socials></Socials>

        
        </div>

        <!-- <div class="about-big w-auto h-auto absolute">
          <h1 class="about-txt">Contact</h1>
        </div> -->
      </section>
    </div>
  </div>
</template>

<script>
import ContactForm from "@/components/Contact/ContactForm";
import Socials from '@/components/Contact/Socials';
export default {
  data() {
      return{

      }
  },
  components: {
    ContactForm,
    Socials
  },
};
</script>

<style lang="less"></style>
