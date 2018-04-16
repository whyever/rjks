<template>
  <div id="app">


    <main>
      <!-- 左侧导航 -->
      <div class="left">

      </div>

      <!-- 右侧主内容区 -->
      <div  class="right" >

        <div class="loginarea">
          <el-row class="username">
            <el-col span="6">
              <p style="color: white">用户名</p>
            </el-col>
            <el-col span="18">
              <el-input
                class="var-username"
                placeholder=""
                v-model="input10"
                clearable>
              </el-input>
            </el-col>
          </el-row>

          <el-row id="password">
            <el-col span="6">
              <p style="color: white">密码</p>
            </el-col>
            <el-col span="18">
              <el-input
                class="var-password"
                placeholder=""
                v-model="input10"
                clearable>
              </el-input>
            </el-col>
          </el-row>

          <div class="block1"></div>

          <el-row class="stu-tch">
            <input type="radio" name="type" style="color: white" value="student" width="50">学生
            <input type="radio" name="type" style="color: white" value="teacher">老师
            <br>
          </el-row>

          <div class="block1"></div>
          <div class="block1"></div>
          <div class="block1"></div>

          <el-row>
            <el-button class="login" type="primary" size="large">登录</el-button>
          </el-row>

        </div>


      </div>
    </main>
  </div>
</template>

<script>
  import Vue from 'vue';
  import ElementUI from 'element-ui';
  import 'element-ui/lib/theme-chalk/index.css';

  Vue.use(ElementUI);

  export default {
    data() {
      return {
        radio:'1'
      }
    }

  }
</script>

<style>
  body{margin: 0;}
  #app {
    min-width: 1200px;
    margin: 0 auto;
    font-family: "Helvetica Neue","PingFang SC",Arial,sans-serif;
  }

  /* 主内容区*/
  main{position: absolute;height: 100%;width: 100%;
    background-image: url("assets/timg.jpg");background-attachment: fixed;background-size: cover;}
  .left{position: absolute;top: 0;left: 0;right: 30%;bottom: 0;overflow: hidden;}
  .right{position: absolute;top:0;right: 0;left: 70%;bottom: 0;background-color: rgba(96, 124, 255, 0.47);}
  .loginarea{position:absolute;top:37%;left: 13%;right: 13%;bottom: 60%;}
  .login{display: block;width: 100%}
  .block1{height: 5px;}
  .stu-tch{color: white}

</style>

