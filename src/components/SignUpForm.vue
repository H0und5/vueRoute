<template>
  <form>
    <label>Email:</label>
    <input type="text" required placeholder="Enter your email" v-model="email" />

    <br /><br />

    <label>Password:</label>
    <input type="text" required placeholder="Enter your password" v-model="password" />

    <button @click.prevent="loginHandler">Login</button>
  </form>
</template>

<script>
import router from '@/router';

  export default {
    data() {
      return {
        email: '',
        password: '',
      }
    },

    methods: {
      loginHandler() {
        console.log(this.email, this.password);

        router.push('/jobs');
      }
    }
  }
</script>

<style>

</style>