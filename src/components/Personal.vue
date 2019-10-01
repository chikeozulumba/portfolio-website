<template>
  <div class="personal-wrapper">
    <div class="personal hT"></div>
    <div class="divider"></div>
    <div id="personal" class="content">
        <h2>Each day would always be my opportunity to become a much better person.<br>I like to talk and make friends at it.</h2>
        <h2>I also enjoy helping people. Even if I haven't travelled the world by now, I still enjoy reading about it.</h2>
        <h2>I also believe that we don't need 'a people' to make change in the this world, but that change actually starts from you.</h2>
        <p class="blockQ">
          These are my philosophies.
        </p>
        <h2>Anyways, when I am not with the code - you can always catch me listening to music or whooping someone at FIFA or NBA.<br><br></h2>
        <div class="social">
          <span>Find me on</span>
          <div class="social-icon">
            <a target="_blank" href="https://twitter.com/chikeozulumba"><img src="/svg/twitter.svg" /></a>
            <a target="_blank" href="https://www.instagram.com/chikeozulumba/"><img style="margin: 0 10px;" src="/svg/instagram.svg" /></a>
            <a target="_blank" href="https://linkedin.com/in/chike-ozulumba-360626b1/"><img src="/svg/linkedin.svg" /></a>
          </div>
        </div>
    </div>
  </div>
</template>

<script>
import Typed from 'typed.js';

export default {
  mounted () {
    setTimeout(() => {
    var typed = new Typed('.personal', {
      strings: ["I'm jovial and open minded.", " I'm Awesome!"],
      typeSpeed: 30,
      backDelay: 1000,
      backSpeed: 10,
    });
    }, 1000);
  }
}
</script>

<style scoped>
.blockQ {
  color: white;
  margin: 50px auto;
  border-top: 1px solid white;
  border-bottom: 1px solid white;
  width: 50%;
  text-align: center;
  padding: 10px;
}
.social {
  color: white;
  margin: 50px auto;
  width: 50%;
  text-align: center;
  padding: 10px;
  display: grid;
  grid-template-columns: 1fr;
  grid-gap: 10px;
}
.social-icon img {
  height: 20px;
}
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
.personal-wrapper {
  padding-right: 10%;
  clear: both;
  max-width: 700px;
  position: absolute;
  top: 30%;
}
.personal-line {
  color: white;
  padding: 20px 0;
}
.hT {
  font-size: 32px;
  color: white;
  line-height: 1.2em;
}
</style>
