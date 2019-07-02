<template>
  <div class="page">
    <div>设计与制作</div>
    <div class="ui-cell animated fadeIn">
      <div class="img_tg ">
        <img
          src="../images/yyfw_1.png"
          alt="设计服务"
          class="img_100 animated fadeIn"
          v-if="indexone"
          @mouseover="checkindex(1,1)"
        >
        <img
          src="../images/yyfw_2.png"
          alt="设计服务"
          class="img_100 animated fadeIn"
          v-else
          @mouseout="checkindex(1,1)"
        >
      </div>
      <div class="img_tg">
        <img
          src="../images/tgfw_1.png"
          alt="制作服务"
          class="img_100 animated fadeIn"
          v-if="indextwo"
          @mouseover="checkindex(2,2)"
        >
        <img
          src="../images/tgfw_2.png"
          alt="制作服务"
          class="img_100 animated fadeIn"
          v-else
          @mouseout="checkindex(2,2)"
        >
      </div>
    </div>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  data() {
    return {
      indexone: true,
      indextwo: true
      //   index2: "2"
    };
  },
  methods: {
    checkindex(state, num) {
      //   console.log(state);
      //   console.log(num);
      if (state == 1) {
        if (num == 1) {
          this.indexone = !this.indexone;
        }
      }
      if (state == 2) {
        if (num == 2) {
          this.indextwo = !this.indextwo;
        }
      }
    }
  },
  components: {}
};
</script>

<style scoped>
.page {
  height: 676px;
  /* width: 1920px; */
  padding-top: 29px;
}
.page > div:first-of-type {
  width: 305px;
  height: 60px;
  font-size: 60px;
  font-weight: bold;
  color: rgba(0, 0, 0, 1);
  margin: 0 auto;
}
.page > div:nth-of-type(2) {
  margin: 0 425px;
  padding-top: 80px;
}
.img_tg {
  height: 423px;
  width: 503px;
  margin: 0 auto;
}
</style>
