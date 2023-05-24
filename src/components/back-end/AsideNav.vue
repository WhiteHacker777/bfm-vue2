<template>
  <div>
    <el-col :span="12">
      <el-menu
          style="width: 200px;height: calc(100vh - 60px)"
          default-active="2"
          class="el-menu-vertical-demo">
        <el-submenu index="1">
          <template slot="title">
            <i class="el-icon-menu"></i>
            <span>用户管理</span>
          </template>
            <el-menu-item index="1-1">选项1</el-menu-item>
            <el-menu-item index="1-2">选项2</el-menu-item>
            <el-menu-item index="1-3">选项3</el-menu-item>
        </el-submenu>

        <el-menu-item index="2">
          <i class="el-icon-menu"></i>
          <span slot="title">书籍管理</span>
        </el-menu-item>

        <el-menu-item index="3">
          <i class="el-icon-menu"></i>
          <span slot="title">电影管理</span>
        </el-menu-item>

        <el-menu-item index="4">
          <i class="el-icon-menu"></i>
          <span slot="title">音乐管理</span>
        </el-menu-item>

        <el-menu-item index="5">
          <i class="el-icon-menu"></i>
          <span slot="title">评论管理</span>
        </el-menu-item>

        <el-menu-item index="6">
          <i class="el-icon-menu"></i>
          <span slot="title">动态管理</span>
        </el-menu-item>

        <el-menu-item index="7">
          <i class="el-icon-menu"></i>
          <span slot="title">小组管理</span>
        </el-menu-item>

      </el-menu>
    </el-col>
  </div>
</template>

<script>
export default {
  name: "AsideNav"
}
</script>

<style scoped>

</style>