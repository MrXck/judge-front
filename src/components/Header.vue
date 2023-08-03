<template>
  <div class="background">
    <div class="header">
      <div class="left">
        <div class="nav">
          <img class="logo" :src="default_avatar" alt="">
<!--          <div class="nav-item">学习</div>-->
          <div class="nav-item">题库</div>
<!--          <div class="nav-item">竞赛</div>-->
<!--          <div class="nav-item">讨论</div>-->
<!--          <div class="nav-item">求职</div>-->
        </div>
      </div>
      <div class="right">
        <div class="nav">
          <img class="avatar nav-item" :src="default_avatar" alt="">
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import default_avatar from '@/assets/default_avatar.png'


</script>

<style scoped>
.background {
  margin: 0 auto;
  height: 50px;
  box-shadow: 0 0 #0000, 0 0 #0000, 0 1px 3px #0000000a, 0 2px 8px #00000014;
  z-index: 10;
}


.header {
  display: flex;
  justify-content: space-between;
  width: 80vw;
  margin: 0 auto;
  height: 100%;
  align-items: center;
  line-height: 22px;
}

.logo {
  width: 20px;
  height: 20px;
  cursor: pointer;
}

.nav {
  display: flex;
}

.nav .nav-item {
  margin-left: 28px;
  cursor: pointer;
  color: #262626bf;
}

.nav .nav-item:hover {
  color: black;
}

.avatar {
  width: 24px;
  height: 24px;
  border-radius: 50%;
  cursor: pointer;
}
</style>