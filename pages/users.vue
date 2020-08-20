<template>
  <div>
    <input type="text" v-model="userID">
    <button @click="onLoadUser">Load user</button>
    <nuxt-child></nuxt-child>
  </div>
</template>

<script>
export default {
  name: "users",
  layout: 'users',
  data() {
    return {
      userID: '',
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userID);
    }
  }
}
</script>

<style scoped>

</style>
