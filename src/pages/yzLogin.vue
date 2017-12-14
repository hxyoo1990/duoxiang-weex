<template>
    <div class="wrapper">
        <head1 title="手机验证码登陆"></head1>
        <inputCell  type="tel" placeholder="请输入手机号码"></inputCell>
        <yzmInput duanxin="true" send="true"></yzmInput>
        <mainButton class="mainButton" txt="验证并登陆"></mainButton>
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
    import  yzmInput from "../components/yzmInput.vue";

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