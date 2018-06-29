<template>
    <div class="container">
        <el-button type="primary" class="btn">All</el-button>
        <el-button type="info" class="btn">To-do</el-button>
        <el-button type="success" class="btn">Done</el-button>
    </div>
</template>

<style lang="scss" scoped>
    .container {
        background: #202020;
        // border: .5px solid #000;
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-items: flex-start;

        .btn {
            width: 100%;
            margin: 0;
            padding: 16px 0;
            border-radius: 0;
        }
    }
</style>

<script>
export default {
    name: 'Aside',
    data () {
        return {

        }
    }
}
</script>