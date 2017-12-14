<template>
    <div class="wrapper">
        <div class="input-box" v-if="duanxin">
            <div class="send-box">
                <image class="image" :src="iconSrc" v-if="icon"></image>
                <input class="input" placeholder="请输入短信验证码"/>
            </div>
            <div class="send-box">
                <text class="chongfa">重发（59）</text>
                <text class="fasong" v-if="send">点击发送</text>
            </div>
        </div>
        <div class="input-box" v-else-if="tupian">
            <div class="send-box">
                <image class="image" :src="iconSrc"></image>
                <input class="input" type="tel" placeholder="请输入图片验证码"/>
            </div>
            <text class="tupian">图片验证码</text>
        </div>
    </div>
</template>

<style scoped>
    .input-box {
        flex-direction: row;
        justify-content: space-between;
        border-bottom-color: #eee;
        border-bottom-style: solid;
        border-bottom-width: 1px;
        padding-right: 26px;
    }

    .image {
        width: 38px;
        height: 48px;
        margin-top: 29px;
        margin-bottom: 26px;
        margin-left: 44px;
        margin-right: 12px;
    }

    .input {
        width: 300px;
        margin-left: 30px;
        margin-top: 42px;
        margin-bottom: 42px;
        font-size: 28px;
        color: #333333;
    }

    .send-box {
        flex-direction: row;
    }

    .chongfa {
        margin-top: 48px;
        font-size: 24px;
        color: #8b8b8d;
    }

    .fasong {
        margin-top: 48px;
        font-size: 24px;
        color: #22bab9;
        margin-left: 44px;
    }

    .tupian {
        margin-top: 42px;
        margin-left: 100px;
    }

</style>

<script>
    export default {
        props: ['iconSrc', 'duanxin', 'tupian', 'icon', 'send']
    }
</script>