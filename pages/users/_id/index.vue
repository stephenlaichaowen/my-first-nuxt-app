<template>
  <div>
    <h1>A single user, with ID: {{ $route.params.id }}</h1>
    <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded" @click="$router.push('/users')">Back</button>
  </div>
</template>

<script>
  export default {
    validate(data) {
      console.log(data)
    }
  }
</script>

<style scoped>

</style>