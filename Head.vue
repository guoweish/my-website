<template>
  <div id='head'>
    <h1>
      {{headName}}
    </h1>
  </div>
</template>

<script>
  // import Vue from 'vue';

  export default {
    data() {
      return {
        headName: "my blog"
      }
    }
  }

  // var instanceData = {
  //   projectsList: [
  //     {
  //       id: 'a',
  //       url: 'xxx'
  //     },
  //     {
  //       id: 'b',
  //       url: 'xxx'
  //     }
  //   ]
  // }

  // new Vue({
  //   el: '#app',
  //   data: instanceData
  // })
</script>

<style>
</style>