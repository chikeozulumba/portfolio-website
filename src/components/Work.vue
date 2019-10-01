<template>
  <div class="work-wrapper">
    <div class="work hT"></div>
    <div class="divider"></div>
    <div id="work" class="content">
        <h2>Backend design for me has to be with PHP, NodeJS, Python, and Go.</h2>
        <!-- <p>In order of strength, PHP and NodeJS any day.</p> -->
        <h2>While, I touch Frontend design once in a while using CSS, SASS, JavaScript, and a host of CSS frameworks.</h2>
        <h2>I am also vast in using different frameworks ranging from React, Laravel, Angular, VueJS, Polymer, and Ionic.</h2>
        <h2>I am member of Developer Communities like <a style="color:#00ef00;" href="https://twitter.com/foorloop">FoorLoop</a>, <a style="color:#f35075" href="https://twitter.com/frontstackio">Frontstackio</a>, <a style="color:#f7c721" href="https://twitter.com/gdglagos">GDG Lagos</a>.</h2>
        <h2>Lastly, I seriously follow guys like <a style="color:#ecf0f1;" href="https://twitter.com/unicodeveloper">Prosper Otemuyiwa</a> and <a style="color:#ecf0f1;" href="https://twitter.com/ireaderinokun">Ire Aderinokun.</a></h2>

        <div class="accomplishments">
          <section>
              <h1>Msaada</h1>
              <h3>Msaada is a native app for keeping fit whilist funding charity organizations.</h3>
              <article>
                  <p>As people walk, run or cycle, Msaada will measure the distance and individuals will earn money for their chosen non-profit.<br>Malta Guinness and its partners will put down an initial 5 million naira<br> for people to run for.<br>Future versions of the app can allow people to donate money that other people can run for.</p>
                  <a href="https://github.com/chikeozulumba/location-stepcounter-on-ionic-3" target="_blank">Check on Github</a>
              </article>
              <!-- <div class="sample" style="transform: translateY(0px);"><img src="img/portfolio_1.png" alt="InteracSMS"></div> -->
          </section>
          <section>
              <h1>Interac SMS</h1>
              <h3>This is a leading bulk SMS platform in Nigeria.<br> Designed for high volume and swift delivery on networks across Nigeria.</h3>
              <article>
                  <p>I developed both front end and backend of this app to provide a better SMS solution in Nigeria. I wrote this in Laravel and VueJS.</p>
                  <a href="http://interacsms.com" target="_blank">Try a demo</a>
              </article>
              <!-- <div class="sample" style="transform: translateY(0px);"><img src="img/portfolio_1.png" alt="InteracSMS"></div> -->
          </section>
          <section>
              <h1>Audio Ads</h1>
              <h3>Mobile Voice Solution with precise audience targeting. Extend your radio commercials on mobile and reach over 15 million in Nigerian audience.</h3>
              <article>
                  <p>I successfully managed <a href="http://www.audioads.com.ng/signup">Audio Ads</a> during my time as a Web Developer at <a href="http://www.wildfusions.com">Wild Fusions</a>.</p>
                  <a href="http://www.audioads.com.ng/signup" target="_blank">Try a demo</a>
              </article>
              <!-- <div class="sample" style="transform: translateY(0px);"><img src="img/portfolio_1.png" alt="InteracSMS"></div> -->
          </section>
          <section>
              <h1>Invoice NG</h1>
              <h3>Go Paperless! Get Paid Faster!! Invoice NG is a simple and easy to use online invoicing software for small business owners & freelancers.</h3>
              <article>
                  <p>I freelanced for the company, innovating around the company's goal and produced live solutions to help the running of the <a href="http://invoice.ng">Invoice NG</a>.</p>
                  <a href="http://invoice.ng/signup" target="_blank">Visit</a>
              </article>
              <!-- <div class="sample" style="transform: translateY(0px);"><img src="img/portfolio_1.png" alt="InteracSMS"></div> -->
          </section>
          <h2 class="bio-st">I have also worked on sweet ideas like IVR Solutions, 2 Way SMS and some other cool projects. <br>I am open to collaborations whether you like me, my work, both or none - I would still be willing to lend a hand. You can send me an email at <a href="mailto:?subject=Hi%20Chike">chike.a.ozulumba@gmail.com</a></h2>
        </div>
    </div>
  </div>
</template>

<script>
import Typed from 'typed.js';

export default {
  mounted () {
    setTimeout(() => {
    var typed = new Typed('.work', {
      strings: ["Denzel Washington would say:", "Luck is when an opportunity comes along and you're prepared for it.", "I am prepared 🤣"],
      typeSpeed: 30,
      backDelay: 1000,
      backSpeed: 10,
    });
    }, 1000);
  }
}
</script>

<style scoped>
@media screen and (max-width: 640px) {
  .accomplishments section {
    padding-right: 0 !important;
  }
}
h2.bio-st {
  color: black !important;
  width: 80%;
  font-size: 16px;
  font-weight: 400;
}
.accomplishments {
  position: absolute;
  margin: 30px 0 0;
  width: 1000px;
  background: white;
  padding: 20px 50px 70px;
  color: #333;
  transform: translateX(-20px);
  -webkit-transform: translateX(-20px);
  border-top-left-radius: 3px;
  border-top-right-radius: 3px;
}
.accomplishments section {
  padding-right: 50%;
  padding-bottom: 35px;
  margin-bottom: 50px;
  border-bottom: dashed 1px black;
  position: relative;
}
.accomplishments p {
  color: #000 !important;
  text-align: left !important;
}
.accomplishments a {
  color: #777 !important;
}
.accomplishments h3 {
  font-weight: 400;
}
@media (max-width: 640px) and (min-width: 320px) {
  .accomplishments {
    width: calc(100% + 20px);
    padding: 10px 20px;
  }
}
h1,
.h1 {
  font-size: 24px;
  color: white;
  line-height: 1.2em;
  margin: 20px 0;
  color: black;
}
h3 {
  font-size: 16px;
  line-height: 1.6;
}
.portfolio section h1 {
  color: #333;
}
div.content {
  width: 95%;
  padding-right: 20px;
}
div.content h2 {
  color: white;
  margin-bottom: 20px;
  font-weight: 400;
}
div.content p {
  color: white;
  margin: 10px 0;
  text-align: center;
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
.work-wrapper {
  padding-right: 10%;
  clear: both;
  max-width: 700px;
  position: absolute;
  top: 30%;
}
.work-line {
  color: white;
  padding: 20px 0;
}
.hT {
  font-size: 32px;
  color: white;
  line-height: 1.2em;
}
</style>
