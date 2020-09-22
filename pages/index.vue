<template>
  <el-row type="flex" justify="center">
    <el-col :md="16" :sm="12">
      <h2 style="text-align: center">Home Page</h2>
      <el-card shadow="never">Tweets</el-card>
    </el-col>
  </el-row>
</template>

<script>
export default {
  head() {
    return {
      title: "Mini Twitter Homepage",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Mini Twitter Homepage",
        },
      ],
    }
  },
}
</script>