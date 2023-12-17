<template>
    <div style="display: flex;line-height: 60px;">
    <div>
        <i class="el-icon-s-fold" style="font-size: 20px;margin-top: 22px;" @click="collapse"></i>
    </div>
    <div style="flex: 1;text-align:center;font-size:34px;">
        <span>欢迎来到超市食品管理系统！</span>
    </div>
        <el-dropdown>
          <span>王小虎     <i class="el-icon-arrow-down" style="margin-right: 5px"></i></span>
          <el-dropdown-menu slot="dropdown">
            <el-dropdown-item @click.native="toUser">个人中心</el-dropdown-item>
            <el-dropdown-item @click.native="logout">退出登录</el-dropdown-item>
          </el-dropdown-menu>
        </el-dropdown>
    </div>
</template>

<script>

    export default {
        name: "Header",
        methods: {
            toUser() {
                console.log("user");
            },
            logout() {
                console.log("logout");
            },
            collapse() {
                this.$emit('doCollapse')
            }
        }
    }
</script>

<style scoped>

</style>