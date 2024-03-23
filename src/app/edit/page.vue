<script setup lang="ts">

</script>
<template>
   <div class="text-wrap">Daftar Mahasiswa</div>
  <n-form-item path="Nim" label="NIM">
      <n-input  placeholder="V3421054"/>
  </n-form-item>
  <n-form-item path="Nama" label="Nama">
      <n-input  placeholder="Yusuf"/>
  </n-form-item>
  <n-form-item path="Alamat" label="Alamat">
      <n-input  placeholder="Kentingan, Jebres"/>
  </n-form-item>
  <n-form-item path="Tanggal_Lahir" label="Tanggal Lahir">
      <n-date-picker></n-date-picker>
  </n-form-item>
  <n-form-item path="Gender" label="Gender">
    <n-select placeholder="laki-laki" />
  </n-form-item>
  <n-form-item path="Usia" label="Usia">
      <n-input placeholder="18"/>
  </n-form-item>
  <n-space>
  <n-button  type="info">Submit</n-button>
  </n-space>
</template>