<template>
    <div class="wrapper">
        <logoHeader></logoHeader>
        <inputCell :iconSrc="inputCell.shoujiLogo" type="tel" placeholder="请输入手机号码" icon="true"></inputCell>
        <inputCell :iconSrc="inputCell.mimaLogo" type="password" placeholder="请输入登陆密码" icon="true"></inputCell>
        <yzmInput :iconSrc="inputCell.yzmLogo" tupian="true"></yzmInput>
        <mainButton class="mainButton" txt="登陆"></mainButton>
        <wjmm txt="忘记密码"></wjmm>
    </div>
</template>

<style scoped>
    .mainButton {
        margin-top: 28px;
    }
</style>

<script>
    import  logoHeader from "../components/logoHead.vue";
    import  inputCell from "../components/input.vue";
    import  yzmInput from "../components/yzmInput.vue";
    import  mainButton from "../components/mainButton.vue";
    import  wjmm from "../components/wjmm.vue";

    export default {
        data(){
            return {
                inputCell: {
                    shoujiLogo:"http://192.168.0.201:8088/images/zc_shouji@2x.png",
                    mimaLogo:"http://192.168.0.201:8088/images/zc_mima@2x.png",
                    yzmLogo:"http://192.168.0.201:8088/images/zc_yaoshi@2x.png"
                },
            }
        },
        components: {
            logoHeader,
            inputCell,
            yzmInput,
            mainButton,
            wjmm,
        }


    }
</script>