<template>
  <div  class="wss-container">
    <el-card>
    <div class="wss-login-box">
      <div class="wss_login_box_title">
        排班系统
      </div>
      <div class="wss_login_box_item">
        <div class="wss_login_box_name">
<el-input placeholder="请输入用户名" v-model="name">
    <template slot="prepend">请输入用户名</template>
  </el-input>
      </div> 
      </div>
      <div class="wss_login_box_item">
      <div class="wss_login_box_password">
     <el-input placeholder="请输入密码" v-model="password">
    <template slot="prepend">请输入密码</template>
  </el-input>
      </div>
      </div>
       <div class="wss_login_box_item loginBtn">
       <el-button type="success" plain @click="toPage">登录</el-button>
       </div>
    </div>
     </el-card>
      </div>

</template>

<script>
export default {
  
   data() {
    return {
      name: '',
      password: '',
    }
  },
 methods:{
   toPage(){
if(this.name==='admin'){
this.$router.push('/adminPage')
}
else{

this.$router.push('/userPage')
}
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
.wss_login_box_item{
  margin:10px;
}
.wss_login_box_title{
text-align: center;
}
.loginBtn{
     display: flex;
  justify-content: center;
  align-items: center;
}
</style>
