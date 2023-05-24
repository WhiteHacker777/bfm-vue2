<template>
  <div style="height: 50px;align-items: center">
    <el-row >
      <el-col :span="4">
        <div class="grid-content bg-purple">
          <span>书籍</span>
        </div>
      </el-col>
      <el-col :span="4" :offset="1">
        <div class="grid-content bg-purple">
          <span style="margin: auto auto">书籍</span>
        </div>
      </el-col>
      <el-col :span="4" :offset="1">
        <div class="grid-content bg-purple">
          <span style="margin: auto auto">书籍</span>
        </div>
      </el-col>
      <el-col :span="4" :offset="1">
        <div class="grid-content bg-purple">
          <span style="margin: auto auto">书籍</span>
        </div>
      </el-col>
      <el-col :span="4" :offset="1">
        <div class="grid-content bg-purple">
          <span style="margin: auto auto">书籍</span>
        </div>
      </el-col>
    </el-row>


<!--      <el-menu-item index="4"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item>-->

  </div>
</template>

<script>
export default {
  name: "Header.vue",
  props:{
    activeIndex:"1",
  },
  methods:{
    handleSelect(){

    }
  }
}
</script>

<style scoped>

</style>