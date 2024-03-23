<script setup lang="ts"></script>

<template>
  <n-space>
  <div class="text-wrap">Daftar Mahasiswa</div>
  </n-space>
  <n-form-item path="Nim" label="NIM">
      <n-input/>
  </n-form-item>
  <n-form-item path="Nama" label="Nama">
      <n-input/>
  </n-form-item>
  <n-form-item path="Alamat" label="Alamat">
      <n-input/>
  </n-form-item>
  <n-form-item path="Tanggal_Lahir" label="Tanggal Lahir">
      <n-date-picker></n-date-picker>
  </n-form-item>
  <n-form-item path="Gender" label="Gender">
    <n-select  />
  </n-form-item>
  <n-form-item path="Usia" label="Usia">
      <n-input/>
  </n-form-item>
  <n-space>
  <n-button  type="info">Submit</n-button>
  <n-button  strong secondary type="tertiary">Edit</n-button>
  </n-space>
</template>
