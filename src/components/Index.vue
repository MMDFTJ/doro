<template>
  <div class="common-layout" style="background-color: rgb(253, 241, 246);min-height: 100vh;">
    <el-container>
      <el-header class="header-container">
        <h1 class="header-large">DORO の 表情包收集站</h1>
        <p class="header-small">收集可爱的 doro 表情包！</p>
        <div style="padding-top: 30px;"><MainDialog /></div>
        <div style="padding-top: 10px;"><SponsorDialog /></div>
      </el-header>

      <el-main class="main-container">
        MAIN
      </el-main>

      <el-footer>Footer</el-footer>
    </el-container>
  </div>
</template>

<script lang="ts" setup>
import Main from './Main.vue'
import MainDialog from './MainDialog.vue'
import SponsorDialog from './SponsorDialog.vue'
</script>

<style scoped>
.header-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 20px 10px;
  height: auto;          /* 取消固定高度 */
  min-height: 100px;     /* 你可以根据需要调整 */
  box-sizing: border-box;
  /* text-align: center; */
  /* background-color: #fff; */
}

.header-large {
  margin: 0;
  font-weight: 700;
  font-size: 35px;
  color: rgb(236, 72, 153);
  word-break: break-word;
}

.header-small {
  margin: 5px 0 0 0;
  font-size: 15px;
  color: rgb(236, 72, 153);
  word-break: break-word;
}

/* 响应式 */
/* @media (max-width: 600px) {
  .header-large {
    font-size: 26px;
  }
  .header-small {
    font-size: 16px;
  }
} */
.el-container,
.el-header,
.el-main,
.el-footer {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }
</style>
