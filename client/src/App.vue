<template>
  <DashboardPage></DashboardPage>
</template>

<script>
import axios from "axios"
import DashboardPage from "./components/DashboardPage"

export default {
  name: "App",
  components: {
    DashboardPage
  },
  methods: {
    fetchUsers() {
      // isi function ini untuk fetch ke https://jsonplaceholder.typicode.com/users
    }
  },
  created() {}
};
</script>

<style scoped>
</style>