<template>
  <div class="body">
    <div>
      td 
      <span>80kg
      </span>
    </div>
    <el-row>
      <el-col :span="6" >d</el-col>
      <el-col :span="6" >t /2.7</el-col>
      <el-col :span="6" >d /2.1</el-col>
      <el-col :span="6" >z </el-col>
    </el-row>
    <el-row>
      <el-col :span="6" >d</el-col>
      <el-col :span="6" >t</el-col>
      <el-col :span="6" >d</el-col>
      <el-col :span="6" >z edit esential</el-col>
    </el-row>
    <el-row>
      <el-col :span="6">morning</el-col> 
      <el-col :span="6">45g</el-col>
      <el-col :span="6">45g</el-col>
    </el-row>
    <el-row>
      <el-col :span="6">launch</el-col>
      <el-col :span="6">45g</el-col>
      <el-col :span="6">45g</el-col>
    </el-row>
    <el-row>
      <el-col :span="6">eing</el-col>
      <el-col :span="6">45g</el-col>
      <el-col :span="6">45g</el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'Plan',
  props: {
    msg: String
  }
}
</script>

<style scoped lang="scss">
.body {
  background-color: #f0f0f0;
  -webkit-box-shadow: 0px 10px 13px -7px #000000, 5px 5px 15px 5px rgba(0,0,0,0); 
  box-shadow: 0px 10px 13px -7px #a1a1a1, 5px 5px 15px 5px rgba(0,0,0,0);
  border-radius: 10px;
  padding: 3%;
  margin-bottom: 10px;
}

.b_red {
  border: solid 1px red;
}

.el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .el-col {
    border-radius: 4px;
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
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
</style>
