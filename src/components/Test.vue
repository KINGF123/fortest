<template>
    <div>
        <h3>自定义 {{name}}</h3>
        <button @click="change">按钮</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            name:1123
        }
    },
    methods: {
        change(){
            this.name = 321
        }
    },
}
</script>

<style lang="less">
    div {
        background-color: cyan;
    }
</style>