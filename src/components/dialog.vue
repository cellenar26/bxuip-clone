<template>
  <div>
    <button id="dialog1" v-on:click="test">예문보기</button>

    <modal v-if="showModal" v-on:close="showModal=false">
      <h3 id="modal-header" slot="header">알림</h3>
      <h4 id="modal-body" slot="body">alert창입니다.</h4>
      <div id="wrap">
      <h4 slot="footer" v-on:click="showModal=false"></h4>
      </div>
    </modal>
    
  </div>
</template>

<script>
import Modal from './common/Modal.vue'
export default {
  data() {
    return {

      showModal : false
    }
  },
  methods : {
    test : function() {
      this.showModal = !this.showModal;
    }
  },
  components : {
    Modal : Modal
  }
}
</script>

<style scoped>
 #wrap {
       display: block;

    font-weight: normal;
    margin: 0;
    padding: 0;
    font-size: 12px;
box-sizing: border-box;
    text-align: center;
  clear: both;
    display: block;
    content: "";
 }
</style>>
