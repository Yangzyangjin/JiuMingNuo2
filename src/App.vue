<template>
  <div id="app">
    <headers></headers>
    <banner></banner>
    <product></product>
    <operating></operating>
    <CaseShow></CaseShow>
    <about></about>
    <friend></friend>
    <buttonend></buttonend>
    <a href="#dingbu">
      <img src="./images/top.png" class="vue_img">
    </a>
  </div>
</template>

<script>
import headers from "@/components/headers";
import banner from "@/components/banner";
import product from "@/components/product";
import operating from "@/components/operating";
import CaseShow from "@/components/CaseShow";
import about from "@/components/about";
import friend from "@/components/friend";
import buttonend from "@/components/buttonend";

export default {
  name: "App",
  components: {
    banner,
    headers,
    product,
    operating,
    CaseShow,
    about,
    friend,
    buttonend
  }
};
</script>

<style>
@import url("./style/flex");
@import url("./style/style");
.vue_img {
  height: 73px;
  width: 73px;
  position: fixed;
  top: 350px;
  right: 10px;
}
#app{
  width: 1920px;
}
</style>
