<template>
  <h1>A single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
export default {
  name: "_id.vue",
  validate(data) {
    return data.params.id == 1;
  }
}
</script>

<style scoped>

</style>
