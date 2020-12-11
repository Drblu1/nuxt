<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  name: "_id.vue",
  validate(data) {
    console.log(data)
    return true
  }
}
</script>

<style scoped>

</style>
