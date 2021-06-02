<template>
  <div>
    <Navbar></Navbar>
    <DashboardPage v-if="currentPage === 'dashboard'"></DashboardPage>
    <AboutPage v-else-if="currentPage === 'about'"></AboutPage>
    <div v-else>
      <h1>404 Page not found</h1>
    </div>
  </div>
</template>

<script>
import axios from "axios"
import Navbar from "./components/Navbar"
import AboutPage from "./components/AboutPage"
import DashboardPage from "./components/DashboardPage"

export default {
  name: "App",
  data () {
    return {
      currentPage: "dashboard"
    }
  },
  components: {
    DashboardPage,
    AboutPage,
    Navbar
  },
  methods: {
    changePage(page) {
      this.currentPage = page
    }
  },
  created() {}
};
</script>

<style scoped>
</style>