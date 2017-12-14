<template>
    <div class="wrapper">
        <head1 title="设置支付密码"></head1>
        <inputCell  type="password" placeholder="请输入新支付密码"></inputCell>
        <inputCell  type="password" placeholder="请再次输入新密码"></inputCell>
        <yzmInput duanxin="true"></yzmInput>
        <mainButton class="mainButton" txt="确认修改"></mainButton>
    </div>
</template>

<style scoped>
    .mainButton {
        margin-top: 60px;
    }
</style>

<script>
    import  head1 from "../components/head1.vue";
    import  inputCell from "../components/input.vue";
    import  mainButton from "../components/mainButton.vue";
    import  yzmInput from  "../components/yzmInput.vue";


    export default {
        data(){
            return {

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