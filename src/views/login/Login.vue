<template>
    <div>
        hello login
    </div>
</template>

<script setup lang="ts">
// import { defineComponent } from 'vue';
// defineComponent({
//     name: "LoginView"
// })

import http from '@/utils/http';
http.post('/users/login', {
    "email": "huangrong@imooc.com",  // 登录邮箱
    "pass": "huangrong" // 登录密码
}).then((res)=>{
    console.log(res.data)
})

</script>

<style scoped lang="scss">

</style>