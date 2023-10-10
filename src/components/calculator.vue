<template>
  <div class="body">

    <el-form ref="form" :model="form" label-width="auto" size="mini">

      <el-form-item label="搜索">
        <el-select v-model="value" filterable placeholder="请选择">
          <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value">
          </el-option>
        </el-select>
      </el-form-item>
      <el-form-item label="输入">
        <el-input v-model="form.name"></el-input>
      </el-form-item>
      <el-form-item label="选项">
        <el-checkbox-group v-model="form.type">
          <el-checkbox label="选项1" name="type"></el-checkbox>
          <el-checkbox label="选项2" name="type"></el-checkbox>
          <el-checkbox label="选项3" name="type"></el-checkbox>
        </el-checkbox-group>
      </el-form-item>
      <el-form-item label="计算方式">
        <el-radio-group v-model="form.resource">
          <el-radio label="质量"></el-radio>
          <el-radio label="营养素"></el-radio>
        </el-radio-group>
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="onSubmit">计算</el-button>
        <el-button type="primary" @click="onSubmit">添加</el-button>
      </el-form-item>
    </el-form>
    <div class="view_box">
      <el-progress type="circle" :percentage="25" :width="50"></el-progress>
      <el-progress type="circle" :percentage="25" :width="50"></el-progress>
      <el-progress type="circle" :percentage="25" :width="50"></el-progress>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Calculator',
  props: {
    msg: String
  },
  data() {
    return {
      radio: '',
      options: [{
        value: '选项1',
        label: '黄金糕'
      }],
      value: '',
      checked: false,
      form: {
        name: '',
        region: '',
        date1: '',
        date2: '',
        delivery: false,
        type: [],
        resource: '',
        desc: ''
      }
    }
  }
}
</script>

<style scoped lang="scss">
.body {
  -webkit-box-shadow: 10px 10px 13px -7px #000000, 5px 5px 15px 5px rgba(0, 0, 0, 0);
  box-shadow: 10px 10px 13px -7px #a1a1a1, 5px 5px 15px 5px rgba(0, 0, 0, 0);
  border-radius: 10px;
  padding: 3%;
  margin-bottom: 10px;
}

.good_input {
  height: 10px;
}

.b_red {
  border: solid 1px red;
}

.m_input {
  width: 200px;
}

.s_input {
  width: 80px;
}

.view_box{
  display: flex;
  justify-content: space-around;
}
</style>
