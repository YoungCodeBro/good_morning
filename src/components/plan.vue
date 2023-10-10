<template>
  <div class="body">
    <el-row>
      <el-col :span="6">当前体重</el-col>
      <el-col :span="6">80kg</el-col>
    </el-row>
    <el-row >
      <el-col :span="6" >摄入标准</el-col>
      <el-col :span="6" >碳水 /2.7</el-col>
      <el-col :span="6" >蛋白质 /2.1</el-col>
      <el-col :span="6" >脂肪 /不计</el-col>
    </el-row>
    <el-row>
      <el-col :span="6" >定量</el-col>
      <el-col :span="6" >145g</el-col>
      <el-col :span="6" >100g</el-col>
      <el-col :span="6" >不计</el-col>
    </el-row>
    <el-row>
      <el-col :span="6">早餐</el-col> 
      <el-col :span="6">45g</el-col>
      <el-col :span="6">45g</el-col>
    </el-row>
    <el-row>
      <el-col :span="6">午餐</el-col>
      <el-col :span="6">45g</el-col>
      <el-col :span="6">45g</el-col>
    </el-row>
    <el-row>
      <el-col :span="6">晚餐</el-col>
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
  -webkit-box-shadow: 0px 10px 13px -7px #000000, 5px 5px 15px 5px rgba(0,0,0,0); 
  box-shadow: 0px 10px 13px -7px #a1a1a1, 5px 5px 15px 5px rgba(0,0,0,0);
  border-radius: 10px;
  padding: 3%;
  margin-bottom: 10px;
}

.b_red {
  border: solid 1px red;
}

.el-col{
  border: solid 1px #ebeef5;
  min-height: 25px;
  line-height: 25px;
}



</style>

