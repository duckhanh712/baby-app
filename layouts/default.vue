<script setup lang="ts">
const titles = [
  { text: 'Hotels & Homes' },
  { text: 'Hotels & Homes' },
  { text: 'Flights' },
  { text: 'Coupons & DealsApartments' },
  { text: 'Apartments', icon: 'mdi-flag' },
]

const items = [
  { title: 'Activities' },
  { title: 'Airport transfer' },
  { title: 'Car rentals' },
]

const topData = {
  hotline: '0354350066',
  totalStore: 679
}

</script>

<template>
  <div class="banner-top bg-rose-100">
    <ul class="content flex gap-x-[28px]">
      <li class="item cursor-pointer">Mua hàng và CSKH: 
        <span class="text hotline"> {{ topData.hotline }} </span>
      </li>
      <li class="item cursor-pointer">Tìm Siêu Thị<span class="text store"> ({{ topData.totalStore }}) </span></li>
      <li class="item cursor-pointer"><span class="mdi mdi-map-marker-outline"></span>Nhập địa chỉ để mua hàng giao <span class="text ship"> Siêu Tốc 1h </span> </li>
      <li class="item cursor-pointer"><span class="mdi mdi-account-supervisor"></span> Đăng nhập</li>
    </ul>
  </div>
  <div class="search-component flex items-center m-auto py-5">
    <div class="w-[20%] flex justify-end	">
      <img class=" w-[134px]" src="https://cdn1.concung.com/themes/desktop4.1/image/logo-concung.png" alt="">
    </div>
    <div>

    </div>
    <div class="search-component relative w-[52%] m-auto">
    <form class="search-form">
      <input class="input focus:outline-none" type="text">
      <button class="search-button" color="primary"></button>
    </form>
    </div>
    <div class="cart-area w-[20%] flex font-bold gap-x-14">
      <div class="cart"><div class="image m-auto"></div><span class="mt-auto">Giỏ hàng</span></div>
      <div class="noti"><div class="image m-auto"></div><span class="mt-auto">Ưu đãi</span></div>
    </div>
  </div>
  <NuxtPage />
</template>

<NuxtPage />
<style lang="scss" scoped>
.banner-top {
  padding: 10px 10%;
  > .content {
    gap: 10%;
    font-size: 14px;
    justify-content: space-between;
  }
}

.search-component {
  max-width: 1600px;
}

.search-form {
  .input {
    width: 92%;
    height: 48px;
    border: 3px solid #ff469e;
    border-radius: 12px 0 0 12px;
    padding: 10px 20px 10px 30px;

  }
  .search-button {
    position: absolute;
    right: 0;
    top: 0;
    bottom: 0;
    width: 72px;
    height: 100%;
    background: #ff469e url(https://cdn1.concung.com/themes/desktop4.1/image/v40/icon/search.svg) no-repeat center center;
    background-size: 28px 28px;
    border-radius: 0 12px 12px 0;
    // width: 60px;
    // background-color: #ff469e;
    // border-radius: 0 12px 12px 0;
  }
}

.cart-area {
  color: #67686c;
  font-size: 14px;
  .cart > .image {
    background: url(https://cdn1.concung.com/themes/desktop4.1/image/v40/icon/cart-top.png) no-repeat top 0 left;
    width: 30px;  
    height: 30px; 
    background-size: contain; 

  }

    .noti > .image {
    background: url(https://cdn1.concung.com/themes/desktop4.1/image/v40/icon/notify-top.png) no-repeat top 0 left;
    width: 30px;
    background-size: contain;
    height: 30px;
  }

}

.banner-top > .content > .item {
  .hotline, .store {
    color: #ff469e ;
  }
  .ship {
    color: '#404040'  !important;
  }
}
</style>
