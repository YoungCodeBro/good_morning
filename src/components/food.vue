<template>
  <div class="body">
    <el-row>
      <el-col :span="8">
        <el-image style="width: 100px; height: 100px" :src="url"></el-image></el-col>
      <el-col :span="16">
        <el-row>
            <el-col :span="8">1</el-col>
            <el-col :span="8">2</el-col>
            <el-col :span="8">3</el-col>
          </el-row>
          <el-row>
            <el-col :span="8">1</el-col>
            <el-col :span="8">2</el-col>
            <el-col :span="8">3</el-col>
          </el-row>
          <el-row>
            <el-col :span="8">1</el-col>
            <el-col :span="8">2</el-col>
            <el-col :span="8">3</el-col>
          </el-row>
          <el-row>
            <el-button type="danger">del</el-button>
          </el-row>
      </el-col>

    </el-row>
  </div>
</template>

<script>
export default {
  name: 'Food',
  props: {
    msg: String
  },
  data() {
    return {
      url: 'https://fuss10.elemecdn.com/e/5d/4a731a90594a4af544c0c25941171jpeg.jpeg'
    }
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

.m_input {
  width: 200px;
}
</style>
