<template>
  <nav class="navbar container navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#">CMS</a>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#" @click="changePage('dashboard')">DashBoard </a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" @click="changePage('about')">About</a>
        </li>
      </ul>
    </div>
    </nav>
</template>

<script>
export default {
  name: "Navbar",
  methods: {
    changePage(page) {
      console.log(page)
      // lakukan emit disini
    }
  }
}
</script>

<style>

</style>