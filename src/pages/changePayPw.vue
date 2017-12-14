<template>
    <div class="wrapper">
        <head1 title="修改支付密码"></head1>
        <inputCell  type="password" placeholder="请输入原密码"></inputCell>
        <inputCell  type="password" placeholder="请输入新密码"></inputCell>
        <inputCell  type="password" placeholder="请再次输入新密码"></inputCell>
        <mainButton class="mainButton" txt="确认修改"></mainButton>
        <wjmm txt="忘记支付密码"></wjmm>

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
    import  wjmm from "../components/wjmm.vue";


    export default {
        data(){
            return {

            }
        },
        components: {
            head1,
            inputCell,
            mainButton,
            wjmm,
        },
        methods: {

        },

    }
</script>