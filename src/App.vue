<template>
  <div id="app">
    <dialogComponent></dialogComponent>
  </div>
</template>

<script>

import dialogComponent from './components/dialog'

export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components : {
    'dialogComponent' : dialogComponent
  }
}
</script>

<style>
#app {
  /* font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale; */
  text-align: center;
  /* color: #147ee9; */
  margin-top: 60px;
}
   #dialog1 {
        width: 130px;
    height: 35px;
    line-height: 35px;
    background: #030709;
    color: #fff;
    border: 1px solid #190508;
 }

 #modal-header {
    color: #1299c1;
  font-size: 16px;
    font-weight: 500;
    line-height: 30px;
    word-break: break-all;
    word-wrap: break-word;
    margin-block-start: 0.83em;
    margin-block-end: 0.83em;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
  display: block;
      box-sizing: border-box;
 }

#modal-body {
      padding: 0;
    line-height: 18px;
    font-size: 14px;
    overflow: auto;
    word-break: break-all;
    word-wrap: break-word;
    color: rgba(10, 9, 9, 0.308);
}
</style>
