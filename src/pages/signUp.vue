<template>
    <div class="wrapper">
        <logoHeader></logoHeader>
        <inputCell :iconSrc="inputCell.shoujiLogo" type="tel" placeholder="请输入手机号码" icon="true"></inputCell>
        <inputCell :iconSrc="inputCell.mimaLogo" type="password" placeholder="请设置登陆密码" icon="true"></inputCell>
        <yzmInput :iconSrc="inputCell.yzmLogo" duanxin="true" icon="true" send="true"></yzmInput>
        <mainButton txt="注册" class="mainButton"></mainButton>
        <wjmm txt="使用微信登陆"></wjmm>
        <footer class="footer"></footer>
    </div>
</template>

<style scoped>
    .wrapper {
        position: absolute;
    }
    .mainButton {
        margin-top: 28px;
    }
</style>

<script>
    import  logoHeader from "../components/logoHead.vue";
    import  inputCell from "../components/input.vue";
    import  yzmInput from "../components/yzmInput.vue";
    import  mainButton from "../components/mainButton.vue";
    import  footer from "../components/footer.vue";
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
            footer,
        }


    }
</script>