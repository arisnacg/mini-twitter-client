<template>
  <el-row type="flex" justify="center">
    <el-col :md="16" :sm="12">
      <h2 style="text-align: center">Login Page</h2>
      <el-card shadow="never">
        <el-form ref="form" :model="form" label-width="120px" label-position="left">
          <el-form-item label="Username">
            <el-input v-model="form.name" type="text" placeholder="Type your username"></el-input>
          </el-form-item>
          <el-form-item label="Password">
            <el-input v-model="form.password" show-password placeholder="Type your password"></el-input>
          </el-form-item>
          <el-form-item>
            <el-button type="primary" @click="login">Login</el-button>
            <el-button @click="$router.push('/register')">Don't account?</el-button>
          </el-form-item>
        </el-form>
      </el-card>
    </el-col>
  </el-row>
</template>

<script>
export default {
  head() {
    return {
      title: "Mini Twitter Login",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Mini Twitter - Login",
        },
      ],
    }
  },
  data() {
    return {
      form: {},
    }
  },
  methods: {
    login() {
      alert("Processing")
    },
  },
}
</script>