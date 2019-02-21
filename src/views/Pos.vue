<template>
  <div class="pos">
    <div>
      <el-row>
        <el-col :span="7" id="order-list">我是订单栏</el-col>
        <!--商品展示-->
        <el-col :span="17">我是产品栏</el-col>
      </el-row>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Pos",
  components: {},
  mounted: function() {
    var orderHeight = document.body.clientHeight;
    document.getElementById("order-list").style.height = orderHeight + "px";
  }
};
</script>
<style scoped>
</style>

