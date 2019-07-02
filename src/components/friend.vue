<template>
  <div class="page">
    <div class="ui-cell ui-cell-cn">
      <img src="../images/hezuo.png">
      <span>合作伙伴</span>
    </div>
    <div>
      <a href="http://www.dianping.com/shop/127001847" target="_black">
        <img src="../images/yeste.png" alt="雅斯特" title="雅斯特">
      </a>
      <a href="http://www.gree.com.cn/" target="_black">
        <img src="../images/geli.png" alt="格力" title="格力">
      </a>
      <a href="http://www.hitachi.com.cn/" target="_black">
        <img src="../images/rili.png" alt="日立" title="日立">
      </a>
      <a href="https://www.viomi.com.cn/" target="_black">
        <img src="../images/ym.png" alt="云米" title="云米">
      </a>
      <a href="http://www.tcl.com/" target="_black">
        <img src="../images/tcl.png" alt="TCL" title="TCL">
      </a>
      <a href="https://www.1688.com/" target="_black">
        <img src="../images/albb.png" alt="阿里巴巴" title="阿里">
      </a>
      <a href="https://www.daikin-china.com.cn/" target="_black">
        <img src="../images/dj.png" alt="大金空调" title="大金">
      </a>
      <a href="https://www.qq.com/" target="_black">
        <img src="../images/tx.png" alt="腾讯" title="腾讯">
      </a>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  data() {
    return {};
  },
  components: {}
};
</script>

<style scoped>
.page {
  /* width: 1116px; */
  height: 592px;
  background: #f3f3f3;
  padding: 0 402px;
  padding-top: 50px;
}
.page > div:nth-of-type(1) > img {
  height: 51px;
  width: 60px;
  padding: 0px;
}
.page > div:nth-of-type(1) > span {
  font-size: 48px;
  font-weight: 400;
  color: rgba(0, 0, 0, 1);
  line-height: 48px;
  margin-left: 19px;
}
.page > div:nth-of-type(2) {
  margin-top: 50px;
}
.page > div:nth-of-type(2) > a > img {
  height: 173px;
  width: 258px;
  margin: 10px;
  border-radius: 8px;
}
.page > div:nth-of-type(2) > a > img:nth-of-type(4n) {
  margin-right: 0px;
}
.page > div:nth-of-type(2) > a > img:nth-of-type(1) {
  margin-left: 0px;
}
.page > div:nth-of-type(2) > img:nth-of-type(5) {
  margin-left: 0px;
}
</style>
