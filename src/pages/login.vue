<template>
    <div class="wrapper">
        <logoHeader></logoHeader>
        <inputCell :iconSrc="input.shoujiLogo" type="tel" placeholder="请输入手机号码" icon="true"></inputCell>
        <inputCell :iconSrc="input.mimaLogo" type="password" placeholder="请输入登陆密码" icon="true"></inputCell>
        <mainButton class="mainButton" txt="登陆" @click="modalSwitch"></mainButton>
        <wjmm txt="忘记密码" @listenToChildEvent="modalSwitch"></wjmm>
        <wjmmModal v-if="showModal" @listenToChildEvent="modalSwitch"></wjmmModal>
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
    import  mainButton from "../components/mainButton.vue";
    import  wjmm from "../components/wjmm.vue";
    import  wjmmModal from "../components/wjmmModal.vue";

    export default {
        data(){
            return {
                input: {
                    shoujiLogo:"http://192.168.0.201:8088/images/zc_shouji@2x.png",
                    mimaLogo:"http://192.168.0.201:8088/images/zc_mima@2x.png",
                },
                showModal: false,
            }
        },
        components: {
            logoHeader,
            inputCell,
            mainButton,
            wjmm,
            wjmmModal,
        },
        methods: {
            modalSwitch() {
                this.showModal= !this.showModal;
            },
        },

    }
</script>