<template>
  <div class="page-container">
    <Navbar />
    <Nuxt />
  </div>
</template>

<script>
import Navbar from "./includes/navbar"
export default {
  components: { Navbar },
}
</script>