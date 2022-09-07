<template>
  <el-form
    label-position="right"
    label-width="100px"
    style="max-width: 460px"
    class="loginForm"
  >
    <el-form-item label="邮箱：">
      <el-input v-model="rEmail" />
    </el-form-item>
    <el-form-item label="密码：">
      <el-input type="password" v-model="rPassword" />
    </el-form-item>
    <el-form-item label="确认密码：">
      <el-input
        type="password"
        v-model="confirmPassword"
        @blur="confirmFunc"
      />
    </el-form-item>
    <el-form-item label="验证码：">
      <el-row>
        <el-input
          type="password"
          v-model="identifyCode"
          class="inpWidth"
        />
        <el-button type="primary" @click="getIdentifyCode" plain>
          获取验证码
        </el-button>
      </el-row>
    </el-form-item>

    <el-row>
      <el-checkbox
        class="checkBox"
        v-model="rAgree"
        label="同意用户使用准则"
        name="type"
      />
    </el-row>
    <el-button
      v-if="rAgree"
      type="primary"
      class="loginBtn"
      @click="register"
    >
      注册
    </el-button>
  </el-form>
</template>

<script>
export default {
  name: "InterviewerLoginComponent"
};
</script>

<style scoped>

</style>