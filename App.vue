<template>
  <div id='app'>
    <ul>
      <li v-for="proj in instanceData" :key="proj.id">
        <!-- <div>{{proj.name}}</div> -->
        <a v-bind:href="proj.url" target="_blank">{{proj.name}} <img v-bind:src="proj.img" /></a>
      </li>
    </ul>

    <HeadComp></HeadComp>
  </div>
</template>

<script>
  import Vue from 'vue';
  import HeadComp from './Head.vue';

  import DataConfig from './DataConfig.js';
  console.log(DataConfig)

  const testImage = require('./statics/github.png');

  export default {
    data() {
      // return {
      //   greeting: "hello world!",
      //   instanceData: [
      //     {
      //       id: 1,
      //       name: "abcdefg",
      //       url: '/projects/proj-noise/',
      //       img: testImage
      //     },
      //     {
      //       id: 2,
      //       name: "hey guys",
      //       url: '/projects/proj-noise/',
      //       img: testImage
      //     }
      //   ]
      // }

      return DataConfig
    },
    components: {
      HeadComp
    }
  }
</script>

<style>
  body {
    /* background-color: black; */
    margin: 0px;
  }
</style>