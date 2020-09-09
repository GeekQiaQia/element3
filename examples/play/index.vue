<template>
  <el-calendar>
  <!-- 这里使用的是 2.5 slot 语法，对于新项目请使用 2.6 slot 语法-->
  <template
    v-slot:dateCell>

    <p>{{slotProps}}</p>
    <!-- <p :class="data.isSelected ? 'is-selected' : ''">
      {{ data.day.split('-').slice(1).join('-') }} {{ data.isSelected ? '✔️' : ''}}{{date}}
    </p> -->
  </template>
</el-calendar>
</template>
<style>
  .is-selected {
    color: #1989FA;
  }
</style>