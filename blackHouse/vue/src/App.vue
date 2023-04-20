<template>
  <div id="app">
    <el-container class="h-100">
      <el-header>
        <Header msg="I'm the head" />
      </el-header>
      <el-container>
        <el-aside width="200px">
          <Aside msg="I'm the Aside" />
        </el-aside>
        <el-container>
          <el-main>
            <Main msg="Im the subject" />
          </el-main>
          <el-footer>
            <Footer msg="Im the Footer" />
          </el-footer>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import Main from "./components/MainE.vue";
import Header from "./components/HeaderE.vue";
import Aside from "./components/AsideE.vue";
import Footer from "./components/FooterE.vue";

export default {
  name: "App",
  components: {
    Main,
    Header,
    Aside,
    Footer,
  },
};
</script>

<style lang="scss">
#app {
  height: 100vh;
}
.h-100 {
  height: 100%;
}
* {
  margin: 0;
  padding: 0;
}
.el-header,
.el-footer {
  padding: 0;
  background-color: #ffffff;
  color: #333;
  text-align: center;
  line-height: 60px;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
  text-align: center;
  line-height: 200px;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}

body > .el-container {
  margin-bottom: 40px;
}

.el-container:nth-child(5) .el-aside,
.el-container:nth-child(6) .el-aside {
  line-height: 260px;
}

.el-container:nth-child(7) .el-aside {
  line-height: 320px;
}
</style>
