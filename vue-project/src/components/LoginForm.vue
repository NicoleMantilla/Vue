<template>
  <div class="home">
<form id="loginForm">
  <input type="name" name="user" placeholder="User" required>
  <input type="password" placeholder="password" name="password" required>
  <button type="submit" >Login</button>
</form>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'LoginForm',
  props: {
    msg: String,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #a6a9e8;
}
</style>
