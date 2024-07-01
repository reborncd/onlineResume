<!--
 * @Author: reborncd
-->
<template>
  <RowContent
    align="right"
    :label="t('jf.name')"
    :label-bold="true"
    :label-width="220"
    :is-wrap="true"
    :is-title="true"
    :text="t('jf.time')" />

  <ListWrap
    :title="t('responsibilities')"
    :list="list"
    inner
    titleSize="base"
    bold />

  <ProMain />
</template>

<script setup lang="ts">
import { computed } from 'vue'
import RowContent from '../../../components/RowContent/RowContent.vue'
import ListWrap from '../../../components/ListWrap/ListWrap.vue'
import ProMain from './ProMain.vue'
import { useI18n } from 'vue-i18n'
const { t } = useI18n()

const list = computed(() => [
  t('jf.r1'),
  t('jf.r2'),
  t('jf.r3'),
  t('jf.r4'),
])
</script>
