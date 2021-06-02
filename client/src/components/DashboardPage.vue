<template>
  <div class="container">
      <h1 class="mb-5">This is Dashboard Page</h1>
      <table class="table">
        <thead>
          <tr>
            <th scope="col">No</th>
            <th scope="col">Email</th>
            <th scope="col">Username</th>
            <th scope="col">Name</th>
          </tr>
        </thead>
        <tbody>
          <!-- lakukan looping komponen UserRow di sini -->
        </tbody>
      </table>
    </div>
</template>

<script>
export default {
  name: "DashboardPage"
}
</script>

<style>

</style>