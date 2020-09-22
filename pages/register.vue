<template>
  <el-row type="flex" justify="center">
    <el-col :md="16" :sm="12">
      <h2 style="text-align: center">Register Page</h2>
      <el-card shadow="never">
        <el-form ref="form" :model="form" label-width="120px" label-position="top">
          <el-form-item label="Username">
            <el-input v-model="form.name" type="text" placeholder="Type your username"></el-input>
          </el-form-item>
          <el-form-item label="Password">
            <el-input v-model="form.password" show-password placeholder="Type your password"></el-input>
          </el-form-item>
          <el-form-item label="Confirm Password">
            <el-input
              v-model="form.confirmPassword"
              show-password
              placeholder="Re-type your password"
            ></el-input>
          </el-form-item>
          <el-form-item>
            <el-button type="primary" @click="register">Register</el-button>
            <el-button @click="$router.push('/login')">Already have account?</el-button>
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
      title: "Mini Twitter - Register",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Mini Twitter - Register",
        },
      ],
    }
  },
  data() {
    return { form: {} }
  },
  methods: {
    register() {},
  },
}
</script>