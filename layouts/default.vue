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
  <div class="">
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
    <div class="search-component h-16 flex items-center">
      <div class="w-[24%] flex justify-end	">
        <img class=" w-[134px]" src="https://cdn1.concung.com/themes/desktop4.1/image/logo-concung.png" alt="">
      </div>
      <form class="search-form width-conten-agoda flex m-auto justify-between">
        <input class="input focus:outline-none" type="text">
        <button class="search-button" color="primary">
          <span class="mdi mdi-magnify"></span>
        </button>
      </form>
      <div class="cart-area w-[20%] flex font-bold gap-x-14">
        <div class="cart"><div class="image m-auto"></div><span class="mt-auto">Giỏ hàng</span></div>
        <div class="noti"><div class="image m-auto"></div><span class="mt-auto">Ưu đãi</span></div>
      </div>
  </div>
  </div>

  <NuxtPage />
</template>

<NuxtPage />
<style lang="scss" scoped>
.border-agoda-pink {
  border: 1px solid rgb(var(--v-theme-agoda-pink));
  border-radius: 5px;
  color: rgb(var(--v-theme-agoda-pink));
}

.border-agoda-pink:hover {
  background-color: rgb(var(--v-theme-agoda-pink));
  color: #fff;
}
.nav-menu {
  font-size: 14px;
}

.banner-top {
  padding: 5px 10%;
  > .content {
    gap: 10%;
    font-size: 14px;
    justify-content: space-between;
  }
}

.search-form {
  .input {
    width: 650px;
    height: 48px;
    border: 2px solid #ff469e;
    border-radius: 12px 0 0 12px;
    padding: 10px;

  }
  .search-button {
    width: 60px;
    background-color: #ff469e;
    border-radius: 0 12px 12px 0;
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
  .text {
    // font-family: HelveticaNeue-Bold;
   
  }
  .hotline, .store {
    color: #ff469e ;
  }
  .ship {
    color: '#404040'  !important;
  }
}
</style>
