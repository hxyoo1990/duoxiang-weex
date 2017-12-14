<template>
    <div class="wrapper">
        <div class="input-box">
            <image class="image" :src="iconSrc" v-if="icon"></image>
            <input class="input"  :type="type" :placeholder="placeholder" />
        </div>
    </div>
</template>

<style scoped>
    .input-box {
        flex-direction: row;
        border-bottom-color: #eee;
        border-bottom-style: solid;
        border-bottom-width: 1px;
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
        width: 400px;
        margin-left: 30px;
        margin-top: 42px;
        margin-bottom: 42px;
        font-size: 28px;
        color: #333333;
     }

</style>

<script>
    export default {
        props:['iconSrc','type','placeholder','icon']
    }
</script>