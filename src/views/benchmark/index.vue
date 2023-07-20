<template>
  <div>
    <h1>New Page</h1>
    <!-- 输入框 -->
    <el-input v-model="input1" placeholder="输入框1" />
    <el-input v-model="input2" placeholder="输入框2" />
    <!-- 复选框 -->
    <el-checkbox v-model="checkbox1">复选框1</el-checkbox>
    <el-checkbox v-model="checkbox2">复选框2</el-checkbox>
    <!-- 提交按钮 -->
    <el-button type="primary" @click="submitForm">提交</el-button>
  </div>
</template>

<script>
export default {
  name: 'Bench',
  data() {
    return {
      input1: '',
      input2: '',
      checkbox1: false,
      checkbox2: false
    }
  },
  methods: {
    submitForm() {
      // 在这里编写提交表单的逻辑
      console.log('提交表单')
    }
  }
}
</script>

<style scoped>
/* 在这里编写新页面的样式 */
</style>
