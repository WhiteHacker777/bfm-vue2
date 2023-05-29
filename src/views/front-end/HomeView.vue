<template>
  <el-container>

    <el-header>
      <Header></Header>
    </el-header>

    <el-container>

      <el-container>

        <el-main>
          Main
          <FilmCard></FilmCard>
          <el-table
              :data="tableData"
              border
              stripe
              style="width: 100%">
            <el-table-column
                prop="date"
                label="日期">
            </el-table-column>
            <el-table-column
                prop="name"
                label="姓名">
            </el-table-column>
            <el-table-column
                prop="address"
                label="地址">
            </el-table-column>
          </el-table>
        </el-main>

        <el-footer>
          页脚
        </el-footer>

      </el-container>


    </el-container>

  </el-container>

</template>

<style>

</style>

<script>
// @ is an alias to /src
import Header from "@/components/front-end/Header";
import FilmCard from "@/components/front-end/FilmCard";

export default {
  name:"Layout",
  components:{
    Header,
    FilmCard,
  },
  data() {
    return {
      tableData: [{
        date: '2016-05-02',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1518 弄'
      }, {
        date: '2016-05-04',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1517 弄'
      }, {
        date: '2016-05-01',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1519 弄'
      }, {
        date: '2016-05-03',
        name: '王小虎',
        address: '上海市普陀区金沙江路 1516 弄'
      }]
    }
  }
}
</script>
