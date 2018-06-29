<template>
    <div class="container">
        <form action="" method="post">
            name: <el-input v-model="input" placeholder="请输入用户名" class="input"></el-input>
            password: <el-input v-model="input" placeholder="请输入密码" class="input"></el-input>
            <el-button type="primary" class="btn">submit</el-button>
        </form>
    </div>
</template>

<style lang="scss" scoped>
    .container {
        width: 300px;
        height: 300px;
        padding: 16px;
        background: #eee;
        // border: 1px solid #010101;
        border-radius: 5px;
        box-shadow: 0 0 5px rgba(0,0,0,1.2);

        .input {
            margin: 10px 0;
        }
        .btn {
            margin: 20px 0;
        }
    }
</style>

<script>
export default {
    name: 'Login',
    data () {
        return {
            input: ''
        }
    }
}
</script>
