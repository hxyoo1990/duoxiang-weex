<template>
    <div class="wrapper">
        <div class="button">
            <text class="txt">{{ txt }}</text>
        </div>
    </div>
</template>

<style scoped>
    .button {
        justify-content: center;
        margin-left: 78px;
        margin-right: 78px;
        border-radius: 100px;
        width: 594px;
        height: 94px;
        background-image: linear-gradient(to right,#a6e27e,#00b4cf);
    }
    .txt {
        text-align: center;
        font-size: 30px;
        color: #ffffff;
    }

</style>

<script>
    export default {
        props:['txt']
    }
</script>