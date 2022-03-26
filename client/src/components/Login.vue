<template>
  <div class="login-container">
    <h1 class="login__title">{{ msg }}</h1>
    <form class="login__form" action="" method="post">
      <div class="login__input-div">
        <label class="login__label">Username: </label>
        <input class="login__input" type="username" />
      </div>
      <div class="login__input-div">
        <label class="login__label">Password: </label>
        <input class="login__input" type="password" />
      </div>
      <button class="login__button">Login</button>
    </form>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";

@Component
export default class Login extends Vue {
  msg = "Please Log In";
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.login-container {
  background-color: #f0f0f0;
  padding: 2rem;
  border-radius: 2rem;
  box-shadow: 0 0.5rem 1em;
  display: flex;
  flex-direction: column;
}

.login__input-div {
  margin: 1rem;
}

.login__label {
  font-weight: bolder;
}

.login__input {
  max-width: 15rem;
}

.login__button {
  background-color: #41b883; /* mint */
  border: none;
  border-radius: 2rem;
  color: white;
  padding: 1rem 3rem;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>
