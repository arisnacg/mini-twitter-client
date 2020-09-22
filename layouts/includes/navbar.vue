<template>
  <el-header style="padding: 0">
    <el-menu :default-active="activeIndex" mode="horizontal">
      <el-menu-item index="1" @click="$router.push('/')">Homepage</el-menu-item>
      <el-menu-item index="2" @click="$router.push('/login')">Login</el-menu-item>
      <el-menu-item index="3" @click="$router.push('/register')">Register</el-menu-item>
    </el-menu>
  </el-header>
  <!-- <header>
    
  </header>-->
</template>

<script>
export default {
  data() {
    return {
      activeIndex: "1",
      listPage: [
        { path: "/", name: "Homepage" },
        { path: "/login", name: "Login" },
        { path: "/register", name: "Regiser" },
      ],
    }
  },
  beforeMount() {
    this.listPage.forEach((e, i) => {
      if (e.path === $nuxt.$route.path) {
        this.activeIndex = `${i + 1}`
        return
      }
    })
  },
}
</script>