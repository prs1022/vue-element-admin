<template>
  <div>
    <!-- 顶部小按钮和输入框的集合 -->
    <div class="top-inputs">
      <el-input size="small" placeholder="小输入框1" />
      <el-button size="small">小按钮1</el-button>
      <el-input size="small" placeholder="小输入框2" />
      <el-button size="small">小按钮2</el-button>
    </div>

    <!-- 宽度较大的输入框和按钮 -->
    <div class="wide-input">
      <el-input placeholder="宽输入框" />
      <el-button>按钮</el-button>
    </div>
  </div>
</template>
<script>
export default {
  name: 'KongMing',
  data() {
    return {
      lineChartData: '123'
    }
  },
  methods: {
    handleSetLineChartData(type) {
      this.lineChartData = '123'
    }
  }
}
</script>

<style scoped>
.top-inputs {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}

.wide-input {
  display: flex;
  align-items: center;
}
.wide-input el-input {
  flex-grow: 1;
  margin-right: 10px;
}
</style>
