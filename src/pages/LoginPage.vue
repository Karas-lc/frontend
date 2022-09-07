<template>
  <div class="layout">
    <el-tabs type="border-card">
      <el-tab-pane label="Candidate">
       <UserLoginComponent/>
      </el-tab-pane>

      <el-tab-pane label="Interviewer">
        <InterviewerLoginComponent />
      </el-tab-pane>
    </el-tabs>
  </div>
</template>

<style scoped>
.layout {
  position: absolute;
  left: calc(50% - 200px);
  top: 20%;
  width: 400px;
}

.loginBtn {
  width: 100px;
}

.loginForm {
  text-align: center;
}

.checkBox {
  margin-left: 7px;
}

.inpWidth {
  width: 165px;
}
</style>


<style scoped>

</style>
<script>
import UserLoginComponent from '../components/auth/CandidateLoginComponent.vue';
import InterviewerLoginComponent from '../components/auth/InterviewerLoginComponent.vue';
export default {
  components: { InterviewerLoginComponent, UserLoginComponent }
}
</script>