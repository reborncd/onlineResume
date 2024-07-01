<!--
 * @Author: reborncd
-->
<template>
  <div class="flex item-center justify-center hover:text-sky-400 dark-transition">
    <Iconfont
      :size="22"
      name="xiazai"
      @click="downloadPdf" /> 
  </div>
</template>

<script setup lang="ts">
import Iconfont from '../../Iconfont/Iconfont.vue'
function downloadPdf() {
  let $el = document.createElement('a')
  $el.href = '../../../../public/常东东-高级前端工程师.pdf'
  $el.target = '_blank'
  $el.download = `常东东-高级前端工程师.pdf`
  document.body.appendChild($el)
  $el.click()
  document.body.removeChild($el)
}
</script>
