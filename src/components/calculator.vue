<template>
  <div class="body">
    <div>
      search
      <el-select v-model="value" filterable placeholder="请选择">
        <el-option v-for="item in options" :key="item.value" :label="item.label" :value="item.value">
        </el-option>
      </el-select>
    </div>
    <div>
      <span>g</span><el-input class="m_input" ></el-input>
    </div>
    <div>
      <span>d</span><el-input class="s_input" ></el-input>
      <span>a</span><el-input class="s_input" ></el-input>
      <span>e</span><el-input class="s_input" ></el-input>
    </div>
    <div>
    radio
      <el-radio v-model="radio" label="1">备选项</el-radio>
      <el-radio v-model="radio" label="2">备选项</el-radio>
    </div>
    <div>
    check
    <el-checkbox v-model="checked">备选项</el-checkbox>
    <el-checkbox v-model="checked">备选项</el-checkbox>
    <el-checkbox v-model="checked">备选项</el-checkbox>
    </div>
    <div>
      <el-button>add</el-button>
    </div>
    <div>
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
        checked: false
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

.s_input {
  width: 80px;
}
</style>
