<template>
    <div class="wrapper">
        <image class="fanhui" src="http://192.168.0.201:8088/images/yz_fanhui@2x.png" resize="cover" style="width:45px;height: 36px" @click="back"></image>
        <text class="title">{{title}}</text>
    </div>
</template>

<style scoped>
    .wrapper {
        flex-direction: row;
        margin-top: 70px;
        margin-bottom: 40px;
    }
    .fanhui {
        padding-left: 26px;
    }
    .title {
        font-size: 32px;
        color: #333;
        margin-left: 218px;
    }



</style>

<script>

    let navigator = weex.requireModule('navigator');

    export default {
        props: ['title'],
        methods: {
            back () {
                navigator.pop({
                    url:'',
                    animated:"true",
                });
            },
        }

    }
</script>