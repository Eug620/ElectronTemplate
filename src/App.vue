<!--
 * @Author       : Eug
 * @Date         : 2021-06-04 18:11:15
 * @LastEditTime : 2021-06-04 18:25:28
 * @LastEditors  : Eug
 * @Descripttion : Descripttion
 * @FilePath     : /vue3-electron/src/App.vue
-->
<script>
import { computed, ref } from 'vue'
export default {
  name: 'App',
  setup() {
    const HelloWrold = ref('Hello World!')
    const useCompHW = computed(() => HelloWrold.value)
    return {
      HelloWrold,
      useCompHW
    }
  }
}
</script>

<template>
  <div class="container mt-2">
    {{ useCompHW }}
  </div>
</template>
