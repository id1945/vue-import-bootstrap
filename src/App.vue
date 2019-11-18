<template>
  <div>
    <div class="text-center mt-5">
      <router-link v-if="loggedIn" to="/logout">Logout</router-link> |
      <router-link to="/login" exact>Login</router-link>
    </div>
    <router-view/>
  </div>
</template>

<script>
export default {
  data () {
    return {
      loggedIn: true
    }
  }
}
</script>
