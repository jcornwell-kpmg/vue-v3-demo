<script>
import UserDetailsForm from "@/components/UserDetails/UserDetailsForm.vue";

export default {
  name: "UserDetails",
  components: { UserDetailsForm },
  props: ["id"],
};
</script>

<template>
  <div id="user-details-screen">
    <nav class="breadcrumb" aria-label="breadcrumbs">
      <ul>
        <li><router-link :to="{ name: 'home' }" class="navbar-item">Home</router-link></li>
        <li class="is-active">
          <!--<a href="#" aria-current="page">User Details</a>-->
          User Details
        </li>
      </ul>
    </nav>

    <UserDetailsForm :user-id="id"></UserDetailsForm>
  </div>
</template>

<style>
#user-details-screen {
  flex: 1 1 auto;
  overflow-y: auto;
  padding: 2rem;
}
</style>