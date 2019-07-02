<template>
  <div class="page" id="CaseShow">
    <div>
      <img src="../images/anlizhanshi.png" class="img_100">
    </div>
    <div class="ui-cell ui-cell-sb">
      <div class="left images">
        <img src="../images/left.png" alt class="img_100" @click="tap(1)">
      </div>
      <div class="page_main animated fadeIn" v-show="issec==1">
        <div class="center">
          <img src="../images/anlidaxiao.png" alt class="img_100">
        </div>
        <div class="text">
          <div>麓明暖通</div>
          <div>
            长沙麓明暖通通过微信小程序抢注名
            称功能，一个月自然访客流量500+
          </div>
          <div>查看更多</div>
        </div>
      </div>
      <div class="page_main animated fadeIn" v-show="issec==2">
        <div class="center">
          <img src="../images/banner2.png" alt class="img_100">
        </div>
        <div class="text">
          <div>长沙暖通</div>
          <div>
            长沙麓明暖通通过微信小程序抢注名
            称功能，一个月自然访客流量500+
          </div>
          <div>查看更多</div>
        </div>
      </div>
      <div class="page_main animated fadeIn" v-show="issec==3">
        <div class="center">
          <img src="../images/banner3.png" alt class="img_100">
        </div>
        <div class="text">
          <div>湖南暖通</div>
          <div>
            长沙麓明暖通通过微信小程序抢注名
            称功能，一个月自然访客流量500+
          </div>
          <div>查看更多</div>
        </div>
      </div>
      <div class="right images">
        <img src="../images/right.png" alt class="img_100" @click="tap(2)">
      </div>
    </div>
    <div class="ui-cell ui-cell-sa opt">
      <ul class="ui-cell">
        <li :class="issec==1 ? 'activeClass' : '' "></li>
        <li :class="issec==2 ? 'activeClass' : '' "></li>
        <li :class="issec==3 ? 'activeClass' : '' "></li>
      </ul>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  data() {
    return {
      issec: 2
    };
  },
  methods: {
    tap(num) {
      if (num === 1) {
        if (this.issec == 1) {
          this.issec = 3;
        } else {
          this.issec = --this.issec;
        }
      }
      if (num === 2) {
        if (this.issec == 3) {
          this.issec = 1;
        } else {
          this.issec = ++this.issec;
        }
      }
    }
  },
  components: {}
};
</script>

<style scoped>
.page {
  /* width: 1920px; */
  height: 1114px;
  background: #e7f6ff;
}
.page > div:nth-of-type(1) {
  height: 90px;
  width: 220px;
  padding-top: 50px;
  margin: 0 auto;
}
.page > div:nth-of-type(2) {
  margin: 0px 305px;
}
.images {
  height: 53px;
  width: 29px;
}
.page_main {
  margin-top: 79px;
}
.center {
  width: 483px;
  height: 841px;
  float: left;
}
.text {
  float: right;
  text-align: right;
  margin-top: 259px;
}
.text > div:nth-of-type(1) {
  font-size: 48px;
  font-weight: bold;
}

.text > div:nth-of-type(2) {
  width: 635px;
  height: 108px;
  font-size: 40px;
  font-weight: 400;
  color: rgba(51, 51, 51, 1);
  line-height: 68px;
}
.text > div:nth-of-type(3) {
  font-size: 48px;
  font-weight: 300;
  border: 2px solid black;
  border-radius: 8px;
  height: 81px;
  width: 230px;
  text-align: center;
  line-height: 81px;
  float: right;
  margin-top: 100px;
}

.opt ul li {
  height: 14px;
  width: 14px;
  background: transparent;
  border: 3px solid #0671bc;
  border-radius: 20px;
  margin: 0 20px;
  position: relative;
  top: -10px;
  left: -320px;
}
.activeClass {
  background: #0671bc !important;
}
</style>
