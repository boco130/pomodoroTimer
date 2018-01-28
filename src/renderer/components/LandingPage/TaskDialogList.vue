<template>
    <el-collapse v-model="activeNames" @change="handleChange">
      <el-collapse-item title="作業済み" name="3">
          <li>作業済みItem1</li>
          <li>作業済みItem2</li>
          <li>作業済みItem3</li>
          <li>作業済みItem4</li>
      </el-collapse-item>
    </el-collapse>
</template>
<script>
  export default {
    data () {
      return {
        activeNames: ['1'],
        checked: false
      }
    },
    methods: {
      handleChange (val) {
        console.log(val)
      }
    }
  }
</script>