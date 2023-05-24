<template>
  <div style="height: 50px;line-height: 50px;border-bottom: 1px solid #cccccc;display: flex">
    <div style="width: 200px;text-align: center;font-weight: bold;color: dodgerblue">后台管理</div>
    <div style="flex: 1"></div>
    <div style="width: 150px">
      <el-dropdown>
        <span class="el-dropdown-link">
          用户姓名<i class="el-icon-arrow-down el-icon--right"></i>
        </span>
        <el-dropdown-menu slot="dropdown">
          <el-dropdown-item>个人信息</el-dropdown-item>
          <el-dropdown-item>退出账号</el-dropdown-item>
        </el-dropdown-menu>
      </el-dropdown>

    </div>
  </div>
</template>


<script>
export default {
  name: "Header"
}
</script>


<style scoped>

.el-dropdown-link {
  cursor: pointer;
  color: #409EFF;
}
.el-icon-arrow-down {
  font-size: 12px;
}

</style>