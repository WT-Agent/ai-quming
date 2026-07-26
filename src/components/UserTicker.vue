<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****9911 生成了新中式香氛品牌 5 个古风雅致名字"
  },
  {
    "text": "用户 186****2200 获得了取自《楚辞》的女宝宝温婉吉名"
  },
  {
    "text": "用户 132****4455 完成了智能机器人公司科技感英文品牌命名"
  },
  {
    "text": "用户 159****7788 生成了独立咖啡馆与品牌一句话 Slogan"
  },
  {
    "text": "用户 175****1122 取得了小红书美学摄影博主高端个性网名"
  }
]);
</script>
