<template>
  <h1>Test vue3</h1>
  <div>
    <div v-if="isVisible">
      Is Visible?
    </div>
    <button @click="isVisible = !isVisible">Toggle Visibility</button>
  </div>
</template>

<script>
import { ref } from 'vue'
export default {
  setup() {
    let isVisible = ref(false)
    return {
      isVisible
    }
  }
}
</script>
