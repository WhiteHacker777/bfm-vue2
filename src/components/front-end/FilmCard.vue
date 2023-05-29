<template>
  <div class="film_card_desp">
    <el-card :body-style="{ padding: '0px' }">
      <div class="film_image">
        <el-image src="https://img1.doubanio.com/view/photo/s_ratio_poster/public/p2887388117.jpg"
                  alt="速度太慢啦"
                  fit="cover">
          <div slot="error" class="image-slot" style="">
            <i class="el-icon-picture-outline"></i>
          </div>
        </el-image>
      </div>
      <div class=""></div>
      <div class="film_desp">
        <el-rate
            v-model="value"
            disabled>
          <span>{{film.name}}</span>
          <span style="text-decoration-color: #ff9900">{{film.value}}</span>
        </el-rate>
      </div>
    </el-card>
  </div>
</template>

<script>
export default {
  name: "ContentCard",
  data() {
    return {
      value: 3.7,
      film:{
        name:'金刚狼',
        value: 3.7,
      }
    }
  }
}
</script>

<style scoped>
.film_card_desp{
  width: 125px;
  height: 220px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, .12), 0 0 6px rgba(0, 0, 0, .04);
}
.film_image{
  width: 125px;
  height: 180px;
  border: black 1px;
}
.film_desp{
  width: 125px;
  height: 40px;
}
</style>