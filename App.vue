<template>
  <div id='app'>
    <ul>
      <li v-for="proj in instanceData" :key="proj.id">
        <!-- <div>{{proj.name}}</div> -->
        <a v-bind:href="proj.url" target="_blank">{{proj.name}}</a>
      </li>
    </ul>

    <HeadComp></HeadComp>

    <h1>
      {{greeting}}
    </h1>
  </div>
</template>

<script>
  import Vue from 'vue';
  import HeadComp from './Head.vue';

  export default {
    data() {
      return {
        greeting: "hello world!",
        instanceData: [
          {
            id: 1,
            name: "abcdefg",
            url: '/projects/proj-noise/'
          },
          {
            id: 2,
            name: "hey guys",
            url: '/projects/proj-noise/'
          }
        ]
      }
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