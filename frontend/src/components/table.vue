<template>
    <el-table 
    :data="fields" max height="1000" border style="width: 100%">
      <el-table-column type="index" width="50" />
      <el-table-column  prop="date" label="Date" width="180" />
      <el-table-column prop="name" label="Name" width="180" />
      <el-table-column  prop="address" label="Address" width="300"/>
    </el-table>
  </template>
  
  <script>

export default {
  name: 'Table',
  props:[
    'fields'
  ]

}
  </script>
  