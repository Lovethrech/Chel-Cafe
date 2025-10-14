<script setup>
import { ref, onMounted, onUnmounted } from 'vue';
import LoadPage from '@/components/LoadPage.vue';
import Auth from '@/components/auth/Auth.vue';

const showComponent = ref(true)
let timeoutId = null
onMounted(() => {
  timeoutId = setTimeout(() => {
    showComponent.value = false
  }, 3000) // 3 seconds
})
onUnmounted(() => {
  clearTimeout(timeoutId)
});
</script>

<template>
  <main>
    <LoadPage 
      v-if="showComponent"
    >
    </LoadPage>
    <Auth 
      v-else
    ></Auth>
  </main>
</template>
