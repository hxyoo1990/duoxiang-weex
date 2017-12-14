<template>
    <div class="wrapper">
        <div class="button-box">
            <div class="button button1" @click="jump('http://192.168.0.201:8088/dist/pages/resetPw.js')">
                <text class="txt">重设密码</text>
            </div>
            <div class="button button2" @click="jump('http://192.168.0.201:8088/dist/pages/yzLogin.js')">
                <text class="txt">手机验证码登陆</text>
            </div>
            <div class="button button3" @click="closeModal">
                <text class="txt cancel">取消</text>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .wrapper {
        position: absolute;
        top: 0;
        left: 0;
        bottom: 0;
        right: 0;
        background-color: #000;
        opacity: .5;
    }
    .button-box {
        align-items: center;
        position: fixed;
        bottom: 0;
        left: 0;
        right:0;
    }
    .button {
        justify-content: center;
        background-color: #ffffff;
        width: 718px;
        height: 132px;
    }
    .button1 {
        border-top-left-radius: 40px;
        border-top-right-radius: 40px;
        border-bottom-color: #eee;
        border-bottom-style: solid;
        border-bottom-width: 1px;
    }

    .button2 {
        border-bottom-left-radius: 40px;
        border-bottom-right-radius: 40px;
    }

    .button3 {
        border-radius: 40px;
        margin-top: 18px;
        margin-bottom: 44px;
    }

    .txt {
        text-align: center;
        font-size: 32px;
    }

    .cancel {
        color: #02d2a6;
    }

</style>

<script>

    let navigator = weex.requireModule('navigator');

    export default {
        methods: {
            closeModal() {
                this.$emit('listenToChildEvent', false);
            },
            jump(_url) {
                navigator.push({
                    url: _url,
                    animated: "false"
                })
            },
        }

    }
</script>