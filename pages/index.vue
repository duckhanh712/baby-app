<script lang="ts" setup></script>

<template>
  <div class="container m-auto">
    <div class="relative">
      <ul class="category font-medium  pl-0 ">
        <li class="flex items-center justify-between"><a href="#">Sữa bột cao cấp</a></li>
        <li class="flex items-center justify-between"><a href="#">Bỉm Tã khuyến mãi</a></li>
        <li class="flex items-center justify-between"><a href="#">Sữa tươi các loại</a></li>
        <li class="flex items-center justify-between"><a href="#">Ăn dặm, dinh dưỡng</a></li>
        <li class="flex items-center justify-between"><a href="#">Vitamin & sức khỏe</a></li>
        <li class="flex items-center justify-between"><a href="#">Chăm sóc gia đình</a></li>
      </ul>
    </div>
  </div>

</template>

<style scoped lang="scss">
.container {
  max-width: 1280px;
  
}
.category {
  color: #67686c;
  font-size: 18px;
  font-family: "HelveticaNeue-Bold" !important;
  width: 225px;
  background-color: rgb(255 228 230);
  > li {
    height: 36px;
    width: 100%;
    line-height: 36px;
    display: inline-block;
    padding-left: 20px;
  }
}

</style>
