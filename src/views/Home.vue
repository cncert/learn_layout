<template>
  <div class="flex-style">
    <el-container>
      <el-header>Header</el-header>
      <el-main>
        <el-container>
          <el-header class="nav">
            <el-row>
              <!--按钮-->
              <el-col :span="3"><div class="grid-content bg-purple"></div></el-col>
              <el-col :span="3"><div class="grid-content bg-purple-purple"></div></el-col>
              <el-col :span="3"><div class="grid-content bg-purple"></div></el-col>
              <el-col :span="3"><div class="grid-content bg-purple-purple"></div></el-col>
              <el-col :span="3"><div class="grid-content bg-purple"></div></el-col>
              <el-col :span="3"><div class="grid-content bg-purple-purple"></div></el-col>
              <el-col :span="3"><div class="grid-content bg-purple"></div></el-col>
              <el-col :span="3"><div class="grid-content bg-purple-purple"></div></el-col>
            </el-row>
          </el-header>
          <el-main>
              <el-row type="flex">
                <!--地图-->
                <el-col :span="16"><div class="grid-content bg-purple chart split-line"></div></el-col>
                <!--线图-->
                <el-col :span="8"><div class="grid-content bg-purple chart"></div></el-col>
              </el-row>
              <el-row type="flex">
              <!--日志-->
                <el-col :span="24"><div class="grid-content bg-purple message"></div></el-col>
              </el-row>
          </el-main>
        </el-container>
      </el-main>
    </el-container>
  </div>
</template>

<script>
//import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.flex-style {
  border: 0px solid #eee;
  display: flex; /* 自适应屏幕高度*/
  min-height: 100vh; /* 自适应屏幕高度*/
  flex-direction: column; /* 自适应屏幕高度*/
}

.el-header, .el-footer {
  padding: 0;
  background-color: #23262e;
  color: #333;
  text-align: center;
  line-height: 8vh;
  height: 8vh !important;
  }
  
.el-main {
  background-color: #E9EEF3;
  color: #333;
  text-align: center;
  padding: 0px;
}

.nav{
  background-color: rgb(62, 50, 104);
  height: 5vh !important;
}

  .el-col {
    border-radius: 0px;
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 0px;
    min-height:5vh;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
  .chart{
    background-color: red;
    height: 60vh;
    
  }
  .split-line{
    border-right: 1px solid 
  }
  .message{
    background-color: yellow;
    height: 27vh;
    border-right: 0px solid
  }
</style>
