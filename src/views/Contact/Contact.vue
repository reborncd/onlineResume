<!--
 * @Author: reborncd
-->
<template>
  <Section
    :title="t('contact.title')"
    icon="lianxi">
    <RowContent
      :label="t('contact.r1')"
      text="18749972854" />
    <RowContent
      :label="t('contact.r2')"
      text="302701088@qq.com/18749972854@163.com" />
    <RowContent
      link
      label="Github"
      text="https://github.com/reborncd" />
    <!-- <RowContent
      link
      :label="t('contact.r4')"
      text="http://blog.fridolph.top" /> -->
  </Section>
</template>

<script setup lang="ts">
import Section from '../../components/Layouts/Section.vue'
import RowContent from '../../components/RowContent/RowContent.vue'
import { useI18n } from 'vue-i18n'
const { t } = useI18n()
</script>
