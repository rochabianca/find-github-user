<template>
  <form @submit.prevent="$emit('submitted', username)">
    <input data-test="search-input" v-model="username" type="text" />
    <button data-test="search-button" type="submit">Submit</button>
  </form>
</template>

<script>
export default {
  name: 'UserSearchForm',
  data() {
    return {
      username: ''
    }
  }
}
</script>

<style>
</style>
