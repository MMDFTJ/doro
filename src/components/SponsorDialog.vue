<template>
  <el-button plain @click="centerDialogVisible = true" style="color: #ffffff;border-color: rgb(251 207 232);background-color: rgb(236 72 153);border-radius: 60px;">
    <el-icon style="font-size: 20px;padding-right: 10px;"><Link /></el-icon>
    赞赏
  </el-button>

  <el-dialog
    v-model="centerDialogVisible"
    title="Doro！~"
    width="500"
    align-center
  >
    
    <span>
      <img src="../images/doro支付.jpg" alt="" style="display: block; margin: 0 auto; width: 280px;">

    </span>
    <template #footer>
      <div class="dialog-footer">
        <!-- <el-button @click="centerDialogVisible = false">Cancel</el-button>
        <el-button type="primary" @click="centerDialogVisible = false">
          Confirm
        </el-button> -->
      </div>
    </template>
  </el-dialog>
</template>

<script lang="ts" setup>
import { ref } from 'vue'

const centerDialogVisible = ref(false)
</script>
