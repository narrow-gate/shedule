<template>
  <div  class="wss-container">
    <el-card>
    <div class="wss-login-box">
      <div class="wss_login_box_title">
        排班系统
      </div>
      <div class="wss_login_box_item">
        <div class="wss_login_box_name">
<el-input placeholder="请输入内容" ></el-input>
<input/>
      </div> 
      </div>
     
      <div class="wss_login_box_password">
        <span>请输入密码：</span>
        <input type="password"/>
      </div>
    </div>
     </el-card> </div>

</template>

<script>
export default {
 methods:{
   topage(){
   this.$router.push('/testPage') 
   }
 }
}
</script>

<style>
.wss-container{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

</style>
