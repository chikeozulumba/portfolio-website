<template>
  <div class="intro-wrapper">
    <div class="intro hT"></div>
    <div class="divider"></div>
    <div id="intro" class="content">
        <h2>As of now, I probably should be working for either Andela, Facebook, Google, or Apple.</h2>
        <h2>If that hasn't happened yet, You can send me a mail @ <a style="color:#00ef00;" href="mailto:chike.a.ozulumba@gmail.com">chike.a.ozulumba@gmail.com</a> to remind me or find out why.</h2>
        <h2>Nevertheless, I love slapping my keyboard each day hoping to change the world.</h2>
    </div>
  </div>
</template>

<script>
import Typed from 'typed.js';

export default {
  head () {
    return {
      title: 'Chike Ozulumba - Professional Software Developer In Lagos Nigeria.',
      meta: [
        { hid: 'description', name: 'description', content: 'About our company Nuxt.js ' }
      ]
    }
  },
  mounted () {
    setTimeout(() => {
    var typed = new Typed('.intro', {
      strings: ["Hi, I am Chike, a Software Developer from Lagos State in Nigeria."],
      typeSpeed: 30
    });
    }, 1000);
  }
}
</script>

<style scoped>
div.content h2 {
  color: white;
  margin-bottom: 20px;
  font-weight: 400;
}
.divider {
  height: 1px;
  background: rgba(255, 255, 255, 0.3);
  width: 100%;
  max-width: 700px;
  margin: 20px 0 50px;
  transition: 0.3s;
  -webkit-transition: 0.3s;
}
.intro-wrapper {
  padding-right: 10%;
  clear: both;
  max-width: 700px;
  position: absolute;
  top: 30%;
}
.intro-line {
  color: white;
  padding: 20px 0;
}
.hT {
  font-size: 32px;
  color: white;
  line-height: 1.2em;
}
</style>
