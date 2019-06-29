<template>
  <div class="user-profile">
    <img
      data-test="user-avatar"
      class="user-profile__avatar"
      :src="user.avatar_url"
      alt="User profile"
    />
    <div data-test="user-name" class="user-profile__name">{{ user.name }}</div>
    <div data-test="user-bio" class="user-profile__bio">{{ user.bio }}</div>
  </div>
</template>

<script>
export default {
  name: 'UserProfile',
  props: {
    user: {
      type: Object,
      required: true,
      default: () => ({})
    }
  }
}
</script>

<style>
</style>
