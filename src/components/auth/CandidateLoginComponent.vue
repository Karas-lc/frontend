<template>
  <el-form
    label-position="right"
    label-width="80px"
    style="max-width: 460px"
    class="loginForm"
  >
    <el-form-item label="Email：">
      <el-input v-model="Email" />
    </el-form-item>
    <el-form-item label="Password：">
      <el-input type="password" v-model="password" />
    </el-form-item>

    <el-button
      type="primary"
      class="loginBtn"
      @click="login"
    >
      登录
    </el-button>
  </el-form>
</template>

<script>
export default {
  name: "UserLoginComponent"
};
</script>

<style scoped>

</style>