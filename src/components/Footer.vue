<template>
  <footer class="footer">
    
    <div class="left">Nuria Oujo</div>
    <div class="right">Contactemos a través de <a href="mailto:oujomiguez.nuria@gmail.com">oujomiguez.nuria@gmail.com</a> o <router-link to="/contact">pulsando aquí</router-link></div>
  </footer>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Footer"
});
</script>

<style scoped lang="less">

@import '../css/variables.less';

.footer {
  background-color: @bodyBgColor;
  width: 100%;
  font-size: 0.8em;
  opacity: 0.7;
  padding-bottom: 30px;
}

.left, .right {
    padding-top: 10px;
    text-align: center;
  }

@media only screen and (min-width: 620px){

  .footer {
    padding: 0;
  }

  .left, .right {
    padding: 20px;
  }

  .left {
    float: left;
  }

  .right {
    float:right;
  }
}
</style>