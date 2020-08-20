<template>
  <h1>Users with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  name: "index",
  validate(data) {
    console.log(data);
    return /^\d+$/.test(data.params.id);
  }
}
</script>

<style scoped>

</style>
