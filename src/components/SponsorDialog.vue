<template>
  <el-button plain @click="centerDialogVisible = true" style="color: rgb(219 39 119);border-color: rgb(251 207 232);">
    <el-icon style="font-size: 20px;padding-right: 10px;"><Link /></el-icon>
    随机表情包 API
  </el-button>

  <el-dialog
    v-model="centerDialogVisible"
    title="API接口"
    width="500"
    align-center
  >
    
    <span>这里是随机表情包API</span>
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
