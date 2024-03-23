<template>
  <div class="flex flex-col space-y-4 ">Daftar Mahasiswa</div>
  <n-form-item path="silahkan cari" label="Silahkan Masukkan Nama">
      <n-input />
    </n-form-item>
  <n-data-table :columns="columns" :data="data" :row-props="rowProps" />
</template>

<script lang="ts">
import { defineComponent, h } from 'vue'
import { NButton } from 'naive-ui'



type RowData = {
  key: number
  nim: string
  name: string
  alamat: string
  tanggal_lahir: string
  gender: string
  usia: string
}
export default defineComponent({
  setup () {
    return {
      rowProps: (row: RowData) => {
        return {
          style: 'cursor: pointer;',
          onClick: () => {
            
          }
        }
      },
      columns: [
        {
          title: 'Nim',
          key: 'nim'
        },
        {
          title: 'Nama',
          key: 'name'
        },
        {
          title: 'Alamat',
          key: 'alamat'
        },
        {
          title: 'Tanggal Lahir',
          key: 'tanggal_lahir'
        },
        {
          title: 'Gender',
          key: 'gender'
        },
        {
          title: 'Usia',
          key: 'usia'
        },
        {
      title: 'Action',
      key: 'actions',
      render (row) {
        return h(
          NButton,
          {
            size: 'small'
          },
          { default: () => 'Hapus' }
        )
      }
    }
      ],
      data: [
        {
          key: 0,
          nim:'V34213654',
          name: 'Yusuf',
          alamat: 'Jalan kentingan RT 05 RW 01 Jebres, Surakarta',
          tanggal_lahir: '20 November 2003',
          gender: 'Laki-laki',
          usia: '18 Tahun'
        },
        {
          key: 1,
          nim:'V34213654',
          name: 'Yusuf',
          alamat: 'Jalan kentingan RT 05 RW 01 Jebres, Surakarta',
          tanggal_lahir: '20 November 2003',
          gender: 'Laki-laki',
          usia: '18 Tahun'
        },
        {
          key: 2,
          nim:'V34213654',
          name: 'Yusuf',
          alamat: 'Jalan kentingan RT 05 RW 01 Jebres, Surakarta',
          tanggal_lahir: '20 November 2003',
          gender: 'Laki-laki',
          usia: '18 Tahun'
        },
      ]
    }
  }
})
</script>