<template>
    <div class="wrapper">
        <text class="txt" @click="openModal">{{ txt }} ></text>
    </div>
</template>

<style scoped>
    .wrapper {
        margin-top: 42px;
        margin-right: 26px;
    }

    .txt {
        text-align: right;
        font-size: 24px;
        color: #8b8b8d;
    }

</style>

<script>
    export default {
        props: ['txt'],
        methods: {
            openModal() {
                this.$emit('listenToChildEvent', true);
            },
        }
    }
</script>