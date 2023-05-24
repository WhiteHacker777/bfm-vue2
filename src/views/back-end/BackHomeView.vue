<template>
  <el-container>

    <el-header>
      <Header></Header>
    </el-header>

    <el-container>

      <el-aside width="200px">
        <aside-nav/>
      </el-aside>

      <el-container>

        <el-main>
          <div style="margin: 10px 0">
<!--            搜索栏-->
            <el-input v-model="search" placeholder="请输入内容" style="width: 20%" clearable></el-input>
            <el-button type="primary" style="margin-left:5px;">搜索</el-button>
<!--            操作栏-->
            <el-button type="primary" style="margin-left:20px;">新增</el-button>
            <el-button type="primary" style="margin-left:20px;">导入</el-button>
            <el-button type="primary" style="margin-left:20px;">导出</el-button>
          </div>

<!--                数据展示栏-->
          <el-table
              :data="tableData"
              border
              stripe
              height="450"
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

<!--            数据展示操作栏-->
            <el-table-column
                fixed="right"
                label="操作"
                width="100">
              <template slot-scope="scope">
                <el-button @click="handleClick(scope.row)" type="text" size="small">编辑</el-button>
                <el-popconfirm
                    title="确定删除此数据吗？"
                    style="margin-left: 5px"
                >
                  <el-button slot="reference" type="text" size="small">删除</el-button>
                </el-popconfirm>
              </template>
            </el-table-column>
          </el-table>


        </el-main>

        <el-footer>
          <!--          分页栏-->
          <div style="margin: auto auto">
            <el-pagination
                @size-change="handleSizeChange"
                @current-change="handleCurrentChange"
                :current-page="currentPage4"
                :page-sizes="[5, 10, 20]"
                :page-size="10"
                layout="total, sizes, prev, pager, next, jumper"
                :total="total">
            </el-pagination>
          </div>
        </el-footer>

      </el-container>


    </el-container>
  </el-container>

</template>

<style>

</style>

<script>
// @ is an alias to /src
import Header from "@/components/back-end/Header";
import AsideNav from "@/components/back-end/AsideNav";

export default {
  name:"Layout",
  components:{
    Header,
    AsideNav,
  },
  data() {
    return {
      search:'',
      tableData: [
          {
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
      }
      ],
      currentPage4:1,
      total:10,
    }
  },
  methods:{
    handleClick(){

    },
    handleSizeChange(){

    },
    handleCurrentChange(){

    },
  }
}
</script>
