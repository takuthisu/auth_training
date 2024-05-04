<script setup lang="ts">
import { Authenticator } from '@aws-amplify/ui-vue'
import '@aws-amplify/ui-vue/styles.css'
</script>

<template>
  <Authenticator :login-mechanisms="['email']">
    <template v-slot="{user, signOut}">
      <img src="./assets/vue.svg">
      <img src="/vite.svg">
      <h1>ログイン成功</h1>
      <h2>{{ user.signInDetails.loginId }}</h2>
      <button @click="signOut">ログアウト</button>
    </template>
  </Authenticator>
</template>
