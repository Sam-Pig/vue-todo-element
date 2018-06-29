<template>
    <div class="container">
        <div class="logoBar">
            <img src="../assets/logo.png" alt="Vue logo"><h2>todo</h2>
            <span>Designed by <a href="https://github.com/Sam-Pig">Sam Pig</a></span>
        </div>
        <div class="functionBar">
            <span>Current user：{{currentVisitor}}</span>
            <el-button type="danger">Log out</el-button>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .container {
        height: 50px;
        padding: 0 16px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        background: #fff;
        // border: 1px solid black;
        box-shadow: 0 0 3px rgba(0,0,0,0.8);

        .logoBar {
            img {
                height: 24px;
                width: 24px;
            }
            h2 {
                display: inline-block;
                margin-right: 8px;
            }
        }

        .functionBar {
            span {
                margin-right: 8px;
            }
        }

    }
</style>

<script>

export default {
    name: 'Header',
    data () {
        return {
            currentVisitor: 'Sam'
        }
    }
}
</script>