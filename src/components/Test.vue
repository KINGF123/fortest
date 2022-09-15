<template>
    <div>
        <h3>自定义 {{name}}</h3>
        <button @click="change">按钮</button>
        <div class="father">
            <div class="son">文字</div>
        </div>
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
    .father {
        position: relative;
        width: 500px;
        height: 500px;
        background-color: red;
        .son {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%,-50%);
            width: 40px;
            height: 40px;
            background-color: yellow;
        }
    }
</style>