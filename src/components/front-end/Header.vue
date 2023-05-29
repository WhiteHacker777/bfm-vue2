<template>
  <div style="align-items: center;background-color: #545c64;text-underline: black">
    <el-row>
      <el-col
          :span="4"
      >
        <div style="width: 200px;text-align: center;font-weight: bold;color: #cccccc;margin-top: 20px;margin-left: 60px">
          书影音社区系统
        </div>

      </el-col>
      <el-col :span="16">
        <div style="display:flex;justify-content:space-around;">
          <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect"
            background-color="#545c64"
            text-color="#fff"
            active-text-color="#ffd04b">
            <el-menu-item index="1">&nbsp;&nbsp;
              <i class="el-icon-film"></i>
              电影&nbsp;&nbsp;</el-menu-item>
            <el-menu-item index="2">&nbsp;&nbsp;
              <i class="el-icon-collection"></i>
              书籍&nbsp;&nbsp;</el-menu-item>
            <el-menu-item index="3">&nbsp;&nbsp;
              <i class="el-icon-headset"></i>
              音乐&nbsp;&nbsp;</el-menu-item>
<!--            <el-submenu index="2">-->
<!--              <template slot="title">&nbsp;&nbsp;音乐&nbsp;&nbsp;</template>-->
<!--              <el-menu-item index="2-1">选项1</el-menu-item>-->
<!--              <el-menu-item index="2-2">选项2</el-menu-item>-->
<!--              <el-menu-item index="2-3">选项3</el-menu-item>-->
<!--            </el-submenu>-->
<!--            <el-submenu index="3">-->
<!--              <template slot="title">&nbsp;&nbsp;书籍&nbsp;&nbsp;</template>-->
<!--              <el-menu-item index="2-4-1">选项1</el-menu-item>-->
<!--              <el-menu-item index="2-4-2">选项2</el-menu-item>-->
<!--              <el-menu-item index="2-4-3">选项3</el-menu-item>-->
<!--            </el-submenu>-->
            <el-menu-item index="4">&nbsp;&nbsp;
              <i class="el-icon-user"></i>
              小组&nbsp;&nbsp;</el-menu-item>
            <el-menu-item index="5">&nbsp;
              <i class="el-icon-s-home"></i>
              个人中心&nbsp;</el-menu-item>
          </el-menu>
        </div>
      </el-col>
      <el-col
          :span="4"
          style="text-align:center"
      >
<!--        <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect"-->
<!--                 background-color="#545c64"-->
<!--                 text-color="#fff"-->
<!--                 active-text-color="#ffd04b"-->
<!--                style="font-size: larger;font-weight: bold">-->
<!--          <el-menu-item index="1">&nbsp;注册&nbsp;</el-menu-item>-->
<!--          <el-menu-item index="2">&nbsp;登录&nbsp;</el-menu-item>-->
<!--        </el-menu>-->
        <el-button round type="info" style="margin-top: 10px" v-if="flag" >登录</el-button>
      </el-col>
<!--      <div class="line"></div>-->
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

    },
    opearLogin(){

    }
  },
  data:function (){
    return{
      flag:true,
    }
  }
}
</script>

<style scoped>

</style>