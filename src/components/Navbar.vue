<template>
  <div class="menu">
    <a class="title" @click.prevent="changeNav('Intro')" href="#">CHIKE ARTHUR OZULUMBA</a>
      <ul class="main-menu">
          <li data-menu="work" class=""><a @click.prevent="changeNav('Work')" href="#work">Work</a></li>
          <li data-menu="personal"><a @click.prevent="changeNav('Personal')" href="#personal">Personal</a></li>
          <li data-menu="chat"><a target="_blank" href="https://api.whatsapp.com/send?phone=2348131976306">Chat</a></li>
      </ul>
      <ul class="right-menu">
          <li><a style="color: rgb(0, 239, 0)" href="mailto:chike.a.ozulumba@gmail.com">chike.a.ozulumba@gmail.com</a></li>
      </ul>
  </div>
</template>

<script>
import {EventBus} from '~/plugins/EventBus';

export default {
  methods : {
    changeNav: function ($) {
      EventBus.$emit('nav', $);
    }
  }
}
</script>

<style scoped>
@media screen and (max-width: 400px) {
  .menu {
    text-align: center;
    padding-left: 5%;
  }
  .main-menu {
    margin: 10px 1% !important;
  }

  .right-menu {
    float: left !important;
  }
  .main-menu li:last-child {
    margin-left: 20px !important;
  }
  .main-menu li:nth-child(2) {
    float: left;
    margin-left: 20px !important;
  }
}
@media screen and (max-width: 737px) {
  .right-menu {
    float: left !important;
  }
}
@media screen and (max-width: 873px) {
  .right-menu {
    float: left !important;
    margin: 10px 0;
  }
}
@media screen and (max-width: 990px) {
  .right-menu {
    float: left !important;
    margin: 10px 0;
  }
}
@media screen and (max-width: 585px) {
  .main-menu {
    padding-left: 0;
    margin: 10px 1% !important;
  }
}
.menu {
  font-family: Sailec;
  margin-bottom: 15%;
  float: left;
  font-size: 14px;
  width: 100%;
}
.menu .title {
  font-size: 16px;
  margin-right: 87px;
}
a {
  text-decoration: none;
  color: white;
}
.title {
  color: white;
  float: left;
  background: white;
  color: black;
  padding: 10px;
  font-family: Boing;
}
.main-menu,
.right-menu {
  padding: 3px 0;
}
.main-menu {
  padding-top: 3px;
  margin-left: 5%;
  float: left;
  margin: 8.5px 50px;
}
.main-menu li:last-child {
  margin-left: 50px;
}
.main-menu li:nth-child(2) {
  float: left;
  margin-left: 50px;
}
li {
  list-style-type: none;
}
.main-menu li:first-child {
  float: left;
}
.main-menu li:last-child {
  float: right;
}
.right-menu {
  float: right;
  margin: 8.5px 0;
}
</style>
