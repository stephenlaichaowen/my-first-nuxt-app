<template>
  <div class="users flex-column">
    <input class="mt-10 appearance-none block w-full bg-white text-gray-700 border border-gray-400 shadow-inner rounded-md py-3 px-4 leading-tight focus:outline-none  focus:border-gray-500" type="text" v-model="userId" @keyup.enter="$router.push('/users/'+userId)" />
    <br>
    <button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded" @click="onLoadUser">Load User</button>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        userId: ''
      }
    },
    methods: {
      onLoadUser() {
        this.$router.push('/users/' + this.userId)
      }
    },
  }
</script>

<style scoped>
.users {
  min-height: 100vh;
  max-width: 500px;
  margin: auto;
}
input {
 
}
</style>