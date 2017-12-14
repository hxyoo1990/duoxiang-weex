<template>
    <div class="wrapper">
        <head1 title="找回密码"></head1>
        <yzmInput duanxin="true"></yzmInput>
        <inputCell  type="password" placeholder="请输入新密码"></inputCell>
        <inputCell  type="password" placeholder="请再次输入新密码"></inputCell>
        <text class="txt">短信验证码已发送至：{{phoneNumber}}</text>
        <mainButton txt="确认修改"></mainButton>
    </div>
</template>

<style scoped>
    .txt {
        margin-top: 25px;
        margin-bottom: 25px;
        text-align: center;
        color: #8b8b8d;
        font-size: 24px;
    }
</style>

<script>
    import  head1 from "../components/head1.vue";
    import  inputCell from "../components/input.vue";
    import  mainButton from "../components/mainButton.vue";
    import  yzmInput from "../components/yzmInput.vue";

    export default {
        data(){
            return {
                phoneNumber:'137****7771',
            }
        },
        components: {
            head1,
            inputCell,
            yzmInput,
            mainButton,
        },
        methods: {

        },

    }
</script>