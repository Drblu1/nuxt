<template>
  <div>
    <input type="text" v-model="userid">
    <button @click="onLoadUser">Load Users</button>
  </div>
</template>

<script>
export default {
  name: "users.vue",
  data() {
    return {
      userid: ''
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userid)
    }
  }
}
</script>

<style scoped>

</style>
