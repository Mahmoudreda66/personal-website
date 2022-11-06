<template>
  <header-vue></header-vue>
  <features-vue></features-vue>
  <div class="container">
    <hr>
  </div>
  <skills-vue></skills-vue>
  <div class="container">
    <hr>
  </div>
  <projects-vue></projects-vue>
  <div class="container">
    <hr>
  </div>
  <download-cv-vue></download-cv-vue>
  <div class="container">
    <hr>
  </div>
  <personal-info-vue></personal-info-vue>
  <div class="container">
    <hr>
  </div>
  <contact-vue></contact-vue>
  <footer-vue></footer-vue>
</template>

<script>

import HeaderVue from './components/Header.vue';
import FeaturesVue from './components/Features.vue';
import SkillsVue from './components/Skills.vue';
import downloadCvVue from './components/downloadCV.vue';
import ProjectsVue from './components/Projects.vue';
import ContactVue from './components/Contact.vue';
import PersonalInfoVue from './components/PersonalInfo.vue';
import FooterVue from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    HeaderVue,
    FeaturesVue,
    SkillsVue,
    downloadCvVue,
    ProjectsVue,
    ContactVue,
    PersonalInfoVue,
    FooterVue
  }
}
</script>

<style lang="scss">
h1.main-theme {
  display: inline-block;
  margin-bottom: 0px;
  font-weight: bold;

  span.text {
    font-size: 30px;
  }

  div:first-of-type {
    margin-top: -15px;

    span.p {
      width: 100%;
      height: 5px;
      display: inline-block;
      background-color: #f44336;

      span {
        width: 5px;
        height: 5px;
        background-color: #fff;
        display: block;
        animation: h1ANimation 1s infinite linear alternate;
      }

      @keyframes h1ANimation {
        from {
          margin-left: 0px;
        }

        to {
          margin-left: 100%;
        }
      }
    }
  }
}

body {
  padding: 0px;
  margin: 0px;
  background-color: #eee;
}

html {
  scroll-behavior: smooth;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
