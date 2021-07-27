<template>
  <div class="opacity-70 hover:opacity-100  cursor-pointer overflow-hidden bg-white bg-opacity-10 rounded " >
    <li class="relative">
      <div class="overflow-hidden w-full group aspect-w-10 aspect-h-7 flex flex-wrap image-hover-zoom">
        <!-- <div class="overlay"> -->
          <img
            :src="require('../../assets/images/' + imageName)"

            class="object-cover pointer-events-none xl:w-96 xl:h-96"
          />
          <!-- <button type="button" class="absolute inset-0">
              <span class="sr-only">View details for IMG</span>
            </button> -->
        </div>
      <!-- </div> -->
    </li>
  </div>
</template>

<script>
export default {
    props:['imageName'],
  data() {
    return {};
  },
};
</script>

<style lang="less">
li {
  width: 100%;
}

.hover {
  background: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 100%;
}

.image-hover-zoom{
   transform: scale(1.0);
   transition: transform .2s ease-in-out;
}

// .img-hover-zoom img {
//   transition: transform .5s ease;
// }

.image-hover-zoom:hover  {
    transition: transform .2s ease-in-out;
  transform: scale(1.1);
}


</style>
