<template>
  <div class="grid grid-cols-1 gap-3 sm:grid-cols-2 md:grid-cols-2 lg:grid-cols-3">
    <RepositoryItem
      name="pythonWebforVideo"
      :description="t('personal.r1')"
      link="https://github.com/reborncd/pythonWebforVideo">
      <div class="flex flex-row">
        <div class="basis-full flex flex-wrap flex-row gap-1">
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E8%AF%AD%E8%A8%80-python-red" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/UI%E6%9E%84%E5%BB%BA%E5%B7%A5%E5%85%B7-gradio-blue" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E5%B7%A5%E5%85%B7-PaddleOCR-blue" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E7%AC%AC%E4%B8%89%E6%96%B9%E5%90%88%E6%88%90-moviepy-blue" />
        </div>
        <a
          class="flex items-center justify-center p-4 cursor-pointer"
          href="https://github.com/reborncd/pythonWebforVideo"
          target="_blank">
          <Iconfont
            name="tiaozhuan"
            :size="22" />
        </a>
      </div>
    </RepositoryItem>

    <RepositoryItem
      name="onlineResume"
      transitionType="fromLeft"
      :description="t('personal.r2')"
      link="https://github.com/reborncd/onlineResume">
      <div class="flex flex-row">
        <div class="basis-full flex flex-wrap flex-row gap-1">
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E8%84%9A%E6%89%8B%E6%9E%B6-vite-red" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E5%89%8D%E7%AB%AF%E6%A1%86%E6%9E%B6-Vue3-%236495ed" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/UI-TailWind-green" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E8%84%9A%E6%9C%AC%E8%AF%AD%E8%A8%80-TypeScript-%25236495ed" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/UI-fri_element_plus-%238a2be2" />
        </div>
        <a
          class="flex items-center justify-center p-4 cursor-pointer"
          href="https://github.com/reborncd/onlineResume"
          target="_blank">
          <Iconfont
            name="tiaozhuan"
            :size="22" />
        </a>
      </div>
    </RepositoryItem>

    <RepositoryItem
      name="my-program"
      :description="t('personal.r3')"
      transitionType="fromTop"
      link="https://github.com/reborncd/workSummary">
      <div class="flex flex-row">
        <div class="flex-1">
          {{ t('personal.recommend') }}
          <a
            class="block"
            target="_blank"
            href="https://fridolph.github.io/my-program/public/hover-transition/transform-effect/index.html"
            >{{ t('personal.r3_t1') }}</a
          >
          <a
            class="block"
            target="_blank"
            href="https://fridolph.github.io/my-program/public/hover-transition/text-hover/index.html"
            >CSS3 text-hover demo</a
          >
        </div>
        <a
          class="flex items-center justify-center p-4 cursor-pointer"
          href="https://github.com/reborncd/workSummary"
          target="_blank">
          <Iconfont
            name="tiaozhuan"
            :size="22" />
        </a>
      </div>
    </RepositoryItem>

    <RepositoryItem
      name="my-element-plus"
      :description="t('personal.r4')"
      transitionType="fromRight"
      link="https://github.com/reborncd/workSummary">
      <div class="flex flex-row">
        <div class="basis-full flex flex-wrap flex-row gap-1">
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E8%84%9A%E6%89%8B%E6%9E%B6-vite-red" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E5%89%8D%E7%AB%AF%E6%A1%86%E6%9E%B6-Vue3-%236495ed" />

          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E8%84%9A%E6%9C%AC%E8%AF%AD%E8%A8%80-TypeScript-%25236495ed" />
          <img
            alt="Static Badge"
            src="https://img.shields.io/badge/%E6%89%93%E5%8C%85%E5%B7%A5%E5%85%B7-Rollup-orange" />
        </div>
        <a
          class="flex items-center justify-center p-4 cursor-pointer"
          href="https://github.com/reborncd/workSummary"
          target="_blank">
          <Iconfont
            name="tiaozhuan"
            :size="22" />
        </a>
      </div>
    </RepositoryItem>

    <!-- 项目虽好，但求面试还写刷面试的，场景过于不适 -->
    <!-- 听取老师建议，PDF把这个效果去掉了 -->
    <!-- 在线简历方便演示估计也没人注意细节暂且保留 -->
    <RepositoryItem
      name="FE-prepare-interview"
      transitionType="fadeIn"
      :description="t('personal.r5')"
      link="https://github.com/reborncd/FE-INTERVIEW">
      <div class="flex flex-row">
        <div class="flex flex-wrap gap-y-2">
          <button class="my-btn">{{ t('personal.b1') }}</button>
          <button class="my-btn">Promise</button>
          <button class="my-btn">{{ t('personal.b3') }}</button>
          <button class="my-btn">http</button>
          <button class="my-btn">{{ t('personal.b5') }}</button>
          <button class="my-btn">{{ t('personal.b6') }}</button>
        </div>
        <a
          class="flex items-center justify-center p-4 cursor-pointer"
          href="https://github.com/reborncd/FE-INTERVIEW"
          target="_blank">
          <Iconfont
            name="tiaozhuan"
            :size="22" />
        </a>
      </div>
    </RepositoryItem>
  </div>
</template>

<script setup lang="ts">
import RepositoryItem from '../../components/RepositoryItem/RepositoryItem.vue'
import Iconfont from '../../components/Iconfont/Iconfont.vue'
import { useI18n } from 'vue-i18n'
const { t } = useI18n()
</script>
