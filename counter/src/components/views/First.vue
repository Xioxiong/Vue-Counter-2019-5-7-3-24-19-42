<template>
  <div class="first-app">
    {{msg}}
    <confirm text="注册" @message="getMessage"></confirm>
  </div>
</template>
<script>
  import Confirm from '../sub/Confirm'
  export default {
    name:"First",
    component:{
      Confirm
    },
    data(){
      return{
        msg:"这是一个傻逼的软件"
      };
    },
    methods:{
      getMessage(val){
        alert(val);
      }
    }
  }
</script>
