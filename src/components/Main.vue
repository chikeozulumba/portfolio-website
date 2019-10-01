<template>
  <div id="root">
    <div class="frame frame-left"></div>
    <div class="frame frame-right"></div>
    <div class="frame frame-top"></div>
    <div class="frame frame-bottom"></div>
    <div id="back-drop"></div>
      <Navbar/>
      <transition
        name="custom-classes-transition"
        enter-active-class="animated fadeInLeft"
        leave-active-class="animated fadeOutRight"
      >
        <component :is="Current"></component>
      </transition>
  </div>
</template>

<script>
import Navbar from './Navbar'
import Intro from './Intro'
import Personal from './Personal'
import Work from './Work'
import {EventBus} from '~/plugins/EventBus';

export default {
  data () {
    return {
      Current: "Intro"
    }
  },
  mounted () {
    EventBus.$on('nav', $ => {
      this.Current = $;
    });
  },
  components: {
    Navbar,
    Intro,
    Personal,
    Work
  }
}
</script>

<style>
@import url(../assets/css/animate.min.css);
@font-face {
  font-family: Sailec;
  src: url(../assets/fonts/Sailec.ttf);
}

@font-face {
  font-family: Boing-Semi;
  src: url(../assets/fonts/Boing-Bold.ttf);
}
* {
  box-sizing: border-box;
}
@font-face {
  font-family: Boing;
  src: url(../assets/fonts/Boing-Semibold.ttf);
}
#root {
  padding: 3% 10%;
}
#main {
  font-family: Sailec;
  background: black;
  /* min-height: 96vh; */
  padding: 50px 5%;
}
body {
  background: black;
  font-family: Sailec, Arial, Helvetica, sans-serif;
  font-size: 16px;
  font-size: 0.8rem;
  font-weight: 400;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
  max-width: 100%;
}
#back-drop {
  position: fixed;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  z-index: -1;
  opacity: 0;
  transition: 1s;
  -webkit-transition: 1s;
  background: #044a6d;
  background-image: linear-gradient(0deg, #00324c 25%, #003a58 100%);
  background-image: -moz-linear-gradient(top, #00324c 25%, #003a58 100%);
  background-image: -webkit-linear-gradient(top, #00324c 25%, #003a58 100%);
  background-image: -o-linear-gradient(top, #00324c 25%, #003a58 100%);
  background-image: -ms-linear-gradient(top, #00324c 25%, #003a58 100%);
}
.frame {
  position: fixed;
  z-index: 100;
  background: white;
}
.frame.frame-left {
  left: 0;
  top: 0;
  height: 100%;
  width: 18px;
}
.frame.frame-right {
  right: 0;
  top: 0;
  height: 100%;
  width: 18px;
}
.frame.frame-top {
  left: 0;
  top: 0;
  height: 100%;
  width: 18px;
}
.frame.frame-bottom {
  left: 0;
  bottom: 0;
  height: 100%;
  width: 18px;
}
</style>
