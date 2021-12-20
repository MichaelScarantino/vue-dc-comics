<template>
  <div id="app">
    <Header />
    <main>
      <div class="container">
        ciao sono un main
      </div>
    </main>
    <Prefooter />
    <Footertop />
    <Footerbottom />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Prefooter from "./components/Prefooter.vue";
import Footertop from "./components/Footertop.vue";
import Footerbottom from "./components/Footerbottom.vue";

export default {
  name: "App",
  components: {
    Header,
    Prefooter,
    Footertop,
    Footerbottom
  },
};
</script>

<style lang="scss">
  @import './style/general.scss';
  @import './style/common.scss';
  @import './style/variables.scss';

  main{

    // TEST
    background-color: chartreuse;
    height: 100px;
  }


</style>
