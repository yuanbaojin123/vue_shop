<template>
    <div class="login">
        <div class="login-container">
            <div class="img">
                <img src="../assets/img/logo.png">
            </div>
            <el-form v-model="form" class="form" ref="form" label-width="0px">
                <el-form-item >
                    <el-input v-model="form.useName" prefix-icon="el-icon-user-solid"></el-input>
                </el-form-item>
                <el-form-item >
                    <el-input v-model="form.password" type="password" prefix-icon="el-icon-s-goods"></el-input>
                </el-form-item>
                <el-form-item class="btn">
                    <el-button type="primary">登入</el-button>
                    <el-button type="info">重置</el-button>
                </el-form-item>
            </el-form>
        </div>
    </div>
</template>

<script>
    export default {
        name: "login",
        data(){
            return{
                form:{
                    useName:"123",
                    password:"dfsdf"
                }
            }
        }
    }
</script>

<style lang="less" scoped>
    .login{
        width: 100%;
        height: 100%;
        background-color: #2e4e6e;
        .login-container{
            width: 450px;
            height: 300px;
            background-color: #ffffff;
            position: absolute;
            left: 50%;
            top:50%;
            transform: translate(-50%,-50%);
            .img{
                width: 100px;
                height: 100px;
                border-radius: 50%;
                position: absolute;
                left: 50%;
                background-color: #ffffff;
                transform: translate(-50%,-50%);
                padding: 10px;
                border: solid 1px #ddd;
                box-shadow: 0 0 10px #eee;
                img{
                    width: 100px;
                    height: 100px;
                    background-color: #eee;
                    border-radius: 50%;
                }
            }
            .form{
                margin-top: 80px;
                padding: 20px;
                .btn{
                    text-align: right;
                }
            }

        }
    }


</style>