<template>
  <header class="header">
    <ul class="nav-items">
      <li>
        <n-link to="/">Home</n-link>
      </li>
      <li>
        <n-link to="/users">Users</n-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style scoped>
.header {
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #ccc;
}

.nav-items {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: 80%;
}

.nav-items a {
  text-decoration: none;
  color: black;
}

.nav-items a:hover,
.nav-items a:active {
  color: white;
}
</style>
