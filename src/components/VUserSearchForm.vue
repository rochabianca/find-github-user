<template>
  <form @submit.prevent="$emit('submitted', username)">
    <el-input
      placeholder="Search the user"
      v-model="username"
      data-test="search-input"
      class="search-form__input"
    >
      <el-button
        data-test="search-button"
        native-type="submit"
        slot="append"
        icon="el-icon-search"
        class="search-form__button"
      ></el-button>
    </el-input>
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
