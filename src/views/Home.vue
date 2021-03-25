<template>
  <div class="home">
    <h1>首页</h1>
  </div>
</template>

<script lang="ts">
import { defineComponent, getCurrentInstance } from 'vue';
import { fetchAccountList } from '@/api/account';
export default defineComponent({
  created() {
    fetchAccountList();
  },
  mounted () {
    fetchAccountList();
  }
});
</script>
