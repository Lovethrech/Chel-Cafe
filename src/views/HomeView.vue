<script setup>
import { ref, onMounted, onUnmounted } from 'vue';
import LoadPage from '@/components/LoadPage.vue';
import Auth from '@/components/auth/Auth.vue';

const showComponent = ref(true)
let timeoutId = null
onMounted(() => {
  timeoutId = setTimeout(() => {
    showComponent.value = false
  }, 10000) // 5 seconds
})
onUnmounted(() => {
  clearTimeout(timeoutId)
});
</script>

<template>
  <main>
    <LoadPage></LoadPage>
    <Auth></Auth>
  </main>
</template>
