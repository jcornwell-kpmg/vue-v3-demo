<script setup>
import UsersList from '@/components/UsersList/UsersList.vue'
</script>

<template>
  <main id="home-screen">
    <h1>Users</h1>
    <UsersList></UsersList>
  </main>
</template>

<style>
#home-screen {
  flex: 1 1 auto;
  overflow-y: auto;
  padding: 2rem;
}

#home-screen h1 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
}
</style>
