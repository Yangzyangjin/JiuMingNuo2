<template>
  <div class="pages">
    <div>
      <ul>
          <li>
            <img
              src="../images/banner1.png"
              alt
              srcset
              class="img_100 animated fadeIn"
              v-show="issec==1"
            >
            <img
              src="../images/banner2.png"
              alt
              srcset
              class="img_100 animated fadeIn"
              v-show="issec==2"
            >
            <img
              src="../images/banner3.png"
              alt
              srcset
              class="img_100 animated fadeIn"
              v-show="issec==3"
            >
          </li>
      </ul>
    </div>
    <div class="ui-cell ui-cell-sa animated fadeIn">
      <ul class="ui-cell">
        <li @click="tap(1)" :class="issec==1 ? 'activeClass' : '' "></li>
        <li @click="tap(2)" :class="issec==2 ? 'activeClass' : '' "></li>
        <li @click="tap(3)" :class="issec==3 ? 'activeClass' : '' "></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      issec: 1
    };
  },
  methods: {
    tap(num) {
      this.issec = num;
    },
    ss() {
      setInterval(()=> {
        var nums = parseInt(Math.random() * 3 + 1, 10);
        this.issec = nums;
        // 不用箭头函数 this指向会有问题
        // console.log("--issec-"+this .issec+"--nums-"+nums);
      }, 4000);
    }
  },
  created() {
    this.ss();
  }
};
</script> 

<style scope>
.pages {
  height: 700px;
  /* width: 1920px; */
}
.pages > div:nth-of-type(1) ul li {
  height: 700px;
  width: 100%
}
.pages > div:nth-of-type(2) ul li {
  height: 14px;
  width: 14px;
  background: transparent;
  border: 3px solid white;
  border-radius: 20px;
  margin: 0 20px;
  position: relative;
  top: -40px;
}
.activeClass {
  background: white !important;
}
</style>  
