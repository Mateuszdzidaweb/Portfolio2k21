<template>
  <div class="w-full h-screen">
    <vue-canvas-nest
      class=""
      :config="{ color: '255,255,255', count: 120 }"
    ></vue-canvas-nest>
    <div class="w-full h-screen flex items-center justify-star">
      <div class="flex flex-col w-auto pl-4">
        <div class="w-auto h-auto flex flex-center pl-2 lg:ml-20">
          <h1 class="text-white text-left title-font swing" v-show="letterVisible1"  v-bind:class="{ bounce: isBounced }">H</h1>
          <h1 class="text-white text-left title-font swing mr-5 effect-shine" v-show="letterVisible2" v-bind:class="{ bounce: isBounced }">i</h1>
        </div>
        <div class="w-auto h-auto flex flex-start py-2 pl-2 lg:ml-20">
          <h1 class="text-white text-left title-font effect-shine swing" v-show="letterVisible3" v-bind:class="{ bounce: isBounced }">M</h1>
          <h1 class="text-white text-left title-font swing mr-3 lg:mr-5" v-show="letterVisible4" v-bind:class="{ bounce: isBounced }">y</h1>

          <h1 class="text-white text-left title-font swing" v-show="letterVisible5" v-bind:class="{ bounce: isBounced }">n</h1>
          <h1 class="text-white text-left title-font swing" v-show="letterVisible6" v-bind:class="{ bounce: isBounced }">a</h1>
          <h1 class="text-white text-left title-font swing" v-show="letterVisible7" v-bind:class="{ bounce: isBounced }">m</h1>
          <h1 class="text-white text-left title-font swing mr-3 lg:mr-5" v-show="letterVisible8" v-bind:class="{ bounce: isBounced }">e</h1>

          <h1 class="text-white text-left title-font swing" v-show="letterVisible9" v-bind:class="{ bounce: isBounced }">i</h1>
          <h1 class="text-white text-left title-font swing mr-3 lg:mr-5" v-show="letterVisible10" v-bind:class="{ bounce: isBounced }">s</h1>

          <h1 class="text-white text-left title-font text swing" v-show="letterVisible11" v-bind:class="{ bounce: isBounced }">M</h1>
          <h1 class="text-white text-left title-font swing" v-show="letterVisible12" v-bind:class="{ bounce: isBounced }">a</h1>
          <span class="text-white text-left title-font swing" v-show="letterVisible13" v-bind:class="{ bounce: isBounced }">t</span>
        </div>

        <div class="w-auto h-auto flex flex-star pl-2  lg:ml-20">
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible14" v-bind:class="{ bounce: isBounced }">I'</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible16" v-bind:class="{ bounce: isBounced }">m</h1>
          <h1 class="text-white text-left title-font  swing ml-3 lg:ml-5" v-show="letterVisible17" v-bind:class="{ bounce: isBounced }">W</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible18" v-bind:class="{ bounce: isBounced }">e</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible19" v-bind:class="{ bounce: isBounced }">b</h1>

          <h1 class="text-white text-left title-font  swing ml-3 lg:ml-5" v-show="letterVisible20" v-bind:class="{ bounce: isBounced }">D</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible21" v-bind:class="{ bounce: isBounced }">e</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible22" v-bind:class="{ bounce: isBounced }">v</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible23" v-bind:class="{ bounce: isBounced }">e</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible24" v-bind:class="{ bounce: isBounced }">l</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible25" v-bind:class="{ bounce: isBounced }">o</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible26" v-bind:class="{ bounce: isBounced }">p</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible27" v-bind:class="{ bounce: isBounced }">e</h1>
          <h1 class="text-white text-left title-font  swing" v-show="letterVisible28" v-bind:class="{ bounce: isBounced }">r</h1>
        </div>

      </div>

      <!-- 
        <h1 class="text-7xl text-white text-left title-font">My name is Mat</h1>
        <h1 class="text-7xl text-white text-left title-font">I'm Web Developer</h1> -->
    </div>
  </div>
</template>

<script>
import vueCanvasNest from "vue-canvas-nest";


export default {
  data() {
    return {
        isBounced: false,
        letterVisible1: false,
        letterVisible2: false,
        letterVisible3: false,
        letterVisible4: false,
        letterVisible5: false,
        letterVisible6: false,
        letterVisible7: false,
        letterVisible8: false,
        letterVisible9: false,
        letterVisible10: false,
        letterVisible11: false,
        letterVisible12: false,
        letterVisible13: false,
        letterVisible14: false,
        letterVisible15: false,
        letterVisible16: false,
        letterVisible17: false,
        letterVisible18: false,
        letterVisible19: false,
        letterVisible20: false,
        letterVisible21: false,
        letterVisible22: false,
        letterVisible23: false,
        letterVisible24: false,
        letterVisible25: false,
        letterVisible26: false,
        letterVisible27: false,
        letterVisible28: false,
    };
  },
  components: { vueCanvasNest },
  created(){
      setTimeout(() => {
        this.letterVisible1 = true
        this.isBounced = true
      }, 1600)
      setTimeout(()=>{
          this.letterVisible2 = true
      },1600)
        setTimeout(()=>{
          this.letterVisible3 = true
      },1700)
        setTimeout(()=>{
          this.letterVisible4 = true
      },1800),
         setTimeout(()=>{
          this.letterVisible5 = true
      },1900)
        setTimeout(()=>{
          this.letterVisible6 = true
      },2000)
        setTimeout(()=>{
          this.letterVisible7 = true
      },2100)
        setTimeout(()=>{
          this.letterVisible8 = true
      },2200),
        setTimeout(()=>{
          this.letterVisible9 = true
      },2300),
        setTimeout(()=>{
          this.letterVisible10 = true
      },2400),
        setTimeout(()=>{
          this.letterVisible11 = true
      },2500)
        setTimeout(()=>{
          this.letterVisible12 = true
      },2600)
        setTimeout(()=>{
          this.letterVisible13 = true
      },2700)
        setTimeout(()=>{
          this.letterVisible14 = true
      },2800),
        setTimeout(()=>{
          this.letterVisible15 = true
      },2900)
        setTimeout(()=>{
          this.letterVisible16 = true
      },3100),
        setTimeout(()=>{
          this.letterVisible17 = true
      },3200),
        setTimeout(()=>{
          this.letterVisible18 = true
      },3300),
        setTimeout(()=>{
          this.letterVisible19 = true
      },3300),
        setTimeout(()=>{
          this.letterVisible20 = true
      },3400),
        setTimeout(()=>{
          this.letterVisible21 = true
      },3500),
        setTimeout(()=>{
          this.letterVisible22 = true
      },3600),
        setTimeout(()=>{
          this.letterVisible23 = true
      },3700),
        setTimeout(()=>{
          this.letterVisible24 = true
      },3800),
              setTimeout(()=>{
          this.letterVisible25 = true
      },3900),
        setTimeout(()=>{
          this.letterVisible26 = true
      },4000),
        setTimeout(()=>{
          this.letterVisible27 = true
      },4100),
        setTimeout(()=>{
          this.letterVisible28 = true
          this.isBounced = false
      },4200),
          setTimeout(()=>{
          this.isBounced = false
      },8000)
      

  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
.vue-canvas-nest-element {
  background-color: #1e1e1e;
  opacity: 1 !important;
}

.title-font {
  font-family: "Ramabhadra", sans-serif;
  font-weight: 700;
  font-size: 3.5vw;
  line-height: 4vw;
  letter-spacing: -1px;
}

.font-size {
}

.bounce{
//   color: #00FDD7;
      animation-duration: 1s;
  animation-fill-mode: both;
  animation-iteration-count: 1;
  animation-name: rubberBand;
}

.text {

    // transform: translate(50%,-50%);
    // text-transform: uppercase;
    font-family: verdana;
   font-size: 3.5vw;
    font-weight: 700;
    color: #1E1E1E;
      -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #00FDD7;
    text-shadow: 1px 1px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 6px 1px #00FDD7,
    1px 18px 6px rgba(16,16,16,0.4),
    1px 22px 10px rgba(16,16,16,0.2),
    1px 25px 35px rgba(16,16,16,0.2),
    1px 30px 60px rgba(16,16,16,0.4);
    ;

        &:hover{
        text-shadow: 1px 1px 1px #919191,
        1px 2px 1px #919191,
        1px 3px 1px #919191,
        1px 4px 1px #919191,
        1px 5px 1px #919191,
        1px 6px 1px #919191,
        1px 7px 1px #919191,
        1px 8px 1px #919191,
        1px 9px 1px #919191,
        1px 10px 1px #919191,
    1px 18px 6px rgba(16,16,16,0.4),
    1px 22px 10px rgba(16,16,16,0.2),
    1px 25px 35px rgba(16,16,16,0.2),
    1px 30px 60px rgba(16,16,16,0.4);
        }
}


// .effect-shine:hover {
//   -webkit-mask-image: linear-gradient(-75deg, rgba(0,0,0,.6) 30%, #000 50%, rgba(0,0,0,.6) 70%);
//   -webkit-mask-size: 200%;
//   animation: shine 2s infinite;
// }

// @-webkit-keyframes shine {
//   from {
//     -webkit-mask-position: 150%;
//   }
  
//   to {
//     -webkit-mask-position: -50%;
//   }
// }

.swing {
  animation-duration: 1s;
  animation-fill-mode: both;
  animation-iteration-count: 1;
}

.swing:hover {
  color: #00FDD7;
  /* animation: rubberBand 5s infinite; */
  animation-name: rubberBand;
}

@keyframes rubberBand {
  from {
    transform: scale3d(1, 1, 1);
  }

  30% {
    transform: scale3d(1.25, 0.75, 1);
  }

  40% {
    transform: scale3d(0.75, 1.25, 1);
  }

  50% {
    transform: scale3d(1.15, 0.85, 1);
  }

  65% {
    transform: scale3d(.95, 1.05, 1);
  }

  75% {
    transform: scale3d(1.05, .95, 1);
  }

  to {
    transform: scale3d(1, 1, 1);
  }
}



@media only screen and (max-width: 1024px) {

  .title-font {
    font-family: "Ramabhadra", sans-serif;
    font-weight: 700;
    font-size: 9.5vw;
     line-height: 10vw;
    letter-spacing: -2px;
  }
  
  .text {

    // transform: translate(50%,-50%);
    // text-transform: uppercase;
    font-family: verdana;
   font-size: 9.5vw;
    font-weight: 700;
    color: #1E1E1E;
      -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #00FDD7;
    text-shadow: 1px 1px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 4px 1px #00FDD7,
        1px 6px 1px #00FDD7,
    1px 18px 6px rgba(16,16,16,0.4),
    1px 22px 10px rgba(16,16,16,0.2),
    1px 25px 35px rgba(16,16,16,0.2),
    1px 30px 60px rgba(16,16,16,0.4);
    ;

        &:hover{
        text-shadow: 1px 1px 1px #919191,
        1px 2px 1px #919191,
        1px 3px 1px #919191,
        1px 4px 1px #919191,
        1px 5px 1px #919191,
        1px 6px 1px #919191,
        1px 7px 1px #919191,
        1px 8px 1px #919191,
        1px 9px 1px #919191,
        1px 10px 1px #919191,
    1px 18px 6px rgba(16,16,16,0.4),
    1px 22px 10px rgba(16,16,16,0.2),
    1px 25px 35px rgba(16,16,16,0.2),
    1px 30px 60px rgba(16,16,16,0.4);
        }
  }

}

@media only screen and (max-width: 600px) {
  .title-font {
    font-family: "Ramabhadra", sans-serif;
    font-weight: 700;
    font-size: 9.5vw;
    line-height: 10vw;
    letter-spacing: -2px;
  }

  .text {

    // transform: translate(50%,-50%);
    // text-transform: uppercase;
    font-family: verdana;
   font-size: 9.5vw;
    font-weight: 700;
    color: #1E1E1E;
      -webkit-text-stroke-width: 2px;
  -webkit-text-stroke-color: #00FDD7;
    text-shadow: 1px 1px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 2px 1px #00FDD7,
        1px 3px 1px #00FDD7,
    1px 18px 6px rgba(16,16,16,0.4),
    1px 22px 10px rgba(16,16,16,0.2),
    1px 25px 35px rgba(16,16,16,0.2),
    1px 30px 60px rgba(16,16,16,0.4);
    ;

        &:hover{
        text-shadow: 1px 1px 1px #919191,
        1px 2px 1px #919191,
        1px 4px 1px #919191,
        1px 4px 1px #919191,
        1px 4px 1px #919191,
        1px 4px 1px #919191,
        1px 4px 1px #919191,
        1px 4px 1px #919191,
        1px 4px 1px #919191,
        1px 5px 1px #919191,
    1px 18px 6px rgba(16,16,16,0.4),
    1px 22px 10px rgba(16,16,16,0.2),
    1px 25px 35px rgba(16,16,16,0.2),
    1px 30px 60px rgba(16,16,16,0.4);
        }
}
}
</style>
