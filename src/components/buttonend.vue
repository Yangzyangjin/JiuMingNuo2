<template>
  <div class="page">
    <div>
      <ul>
        <li>
          <a href="#">门头牌匾</a>
        </li>
        <li>
          <a href="#">亮化工程</a>
        </li>
        <li>
          <a href="#">精简装订</a>
        </li>
        <li>
          <a href="#">雕刻广告</a>
        </li>
        <li>
          <a href="#">高速出图</a>
        </li>
        <li>
          <a href="#">工地广告</a>
        </li>
      </ul>
    </div>
    <div>
      <span>贵州玖铭诺图文广告有限公司  统一社会信用代码 91520103MA6H7BW649</span>
    </div>
    <div>
      <span>版权所有 2018-◎All Rights Reserved.</span>
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
  height: 150px;
  /* width: 1920px; */
  margin: 0 auto;
  text-align: center;
  background: #444545;
  /* padding-top: 20px; */
}
.page > div:nth-of-type(1) ul li {
  display: inline;
}
.page > div:nth-of-type(1) ul li a {
  text-decoration: none;
  display: inline-block;
  padding: 25px 10px;
  color: rgba(255, 255, 255, 1);
  font-size: 18px;
}
.page > div:nth-of-type(1) ul li a:hover {
  color: #278ed7;
}
.page > div:nth-of-type(2) {
  font-size: 18px;
  color: rgba(255, 255, 255, 1);
}
.page > div:nth-of-type(3) {
  font-size: 14px;
  color: rgba(255, 255, 255, 1);
  position: relative;
  bottom: -30px;
}
</style>
