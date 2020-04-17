<template>
  <div class="section section-basic" id="basic-elements">
    <div class="container">
      <h3 class="title">Skills</h3>
      <h4>Technical Skills </h4>
      <div class="row">
        <div class="col-md-12">
          <n-button class="skill" type="primary" size="lg">HTML & CSS</n-button>         
          <n-button class="skill" type="primary" size="lg">BOOTSTRAP</n-button> 
          <n-button class="skill" type="primary" size="lg">JAVASCRIPT</n-button> 
          <n-button class="skill" type="primary" size="lg">VUE.JS</n-button> 
          <n-button class="skill" type="primary" size="lg">NUXT.JS</n-button> 
          <n-button class="skill" type="primary" size="lg">SASS & LESS</n-button> 
          <n-button class="skill" type="primary" size="lg">WORDPRESS</n-button> 
          <n-button class="skill" type="primary">VERSION CONTROL / GIT</n-button>
          <n-button class="skill" type="primary">SEO / GOOGLE ANALYTICS</n-button>
          <n-button class="skill" type="primary">FIGMA</n-button>
          <n-button class="skill" type="primary">PHP</n-button>
          <n-button class="skill" type="primary" size="sm">REACT</n-button>
          <n-button class="skill" type="primary" size="sm">NODE.JS</n-button>
          <n-button class="skill" type="primary" size="sm">TESTING / DEBUGGING</n-button>
        </div>
      </div>
      <br />
      <h4>Non-Technical Skills </h4>
      <div class="row">
        <div class="col-md-12">
          <n-button class="skill" type="primary" size="lg">PROBLEM SOLVING</n-button>         
          <n-button class="skill" type="primary" size="lg">TEAM WORK</n-button> 
          <n-button class="skill" type="primary" size="lg">VOCAL / VERBAL COMMUNICATION</n-button> 
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import {
  Button,
} from '@/components';

export default {
  components: {
    [Button.name]: Button,
  },
  };
</script>
<style>
.skill{
  margin: 10px;
}
</style>
