<template>
  <div class="container">
    <form @submit.prevent="login">
      <div class="row">
        <div class="col-6 m-auto">
          <h2>Login</h2>
          <div class="form-group">
            <label>Email</label>
            <input type="text" class="form-control" v-model="email" placeholder="email"><br />
          </div>
          <div class="form-group">
            <label>Password</label>
            <input type="password" class="form-control" v-model="password" placeholder="password">(hint: password123)<br />
          </div>
          <button type="submit">Login</button>
          <button type="button" @click="setColor">Test Jquery</button>
          <button type="button" data-toggle="popover" data-placement="top" title="Popover on top">Popover on top</button> <!-- /Bootstrap Popover -->
        </div>
      </div>
    </form>
  </div>
</template>

<script>
import $ from "jquery";
export default {
  data () {
    return {
      email: 'test@test.com',
      password: 'Admin@000',
      err: false
    }
  },
  methods: {
    login () {
      alert(`{ email: ${this.email}, password: ${this.password}}`);
    },
    // test jquery
    setColor () {
      $("h2").css({"background-color": "red", "font-size": "200%"});
    }
  },
  mounted() {
    // test popper
    $(function() {
      $('[data-toggle="popover"]').popover()
    });
  }
}
</script>
