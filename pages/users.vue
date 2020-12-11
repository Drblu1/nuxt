<template>
  <div>
    <input type="text" v-model="userid">
    <button @click="onLoadUser">Load Users</button>
    <nuxt-child/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userid: ''
    }
  },
  methods: {
    onLoadUser() {
      this.$router.push('/users/' + this.userid)
    }
  },
  layout: 'users'
}
</script>

<style scoped>

</style>
