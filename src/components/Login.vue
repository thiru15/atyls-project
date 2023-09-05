<template>
  <div class="login-wrapper">
    <div class="logo">
      <img src="./assets/logo.svg" />
    </div>
    <div class="login-card">
      <span id="welcome-message"> WELCOME BACK</span>
      <span class="login-message">Log into your account</span>

      <div>
        <label class="input-box" for="email"> Email or Username </label>
        <input
          type="text"
          placeholder="Enter your email or username"
          id="email"
          name="email"
        />
      </div>

      <div>
        <label class="input-box" for="password"> Password </label>
        <input
          type="text"
          id="password"
          name="password"
          placeholder="Enter your password"
        />
      </div>
      <div>
        <button class="login-button">Login now</button>
      </div>
      <label
        >Not registered yet?
        <span style="color: white"> Register →</span></label
      >
    </div>
  </div>
</template>

<script>
import Vue from "vue";
import Component from "vue-class-component";
// import StarRating from "./components/StarRating";

// Define the component in class-style
@Component({
  name: "Login",
  components: {},
})
export default class Login extends Vue {}
</script>

<style lang="scss" scoped>
.input-box {
  color: #C5C7CA;
  display: flex;
  margin-left: 20px;
}
.login-button {
  width: 415px;
  height: 43px;
  flex-shrink: 0;
  border-radius: 4px;
  background: #4A96FF;
  color: white;
}
.login-wrapper {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}
.logo {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 10%;
  padding-bottom: 30px;
}
.login-card > * {
  display: block;
}
.login-card > * {
  margin-top: 20px;
}
.login-card {
  width: 463px;
  height: 420px;
  flex-shrink: 0;
  border-radius: 8px;
  border: 2px solid #969696;
  background: #27292D;
}
#welcome-message {
  margin-top: 40px;
  color: #6B6C70;
  font-family: Inter;
  font-size: 14px;
  font-style: normal;
  display: block;
  font-weight: 500;
  line-height: normal;
  letter-spacing: 0.42px;
}
.login-message {
  color: #FFF;
  font-family: Inter;
  font-size: 18px;
  font-style: normal;
  display: block;
  font-weight: 600;
  line-height: normal;
}
input > * {
  border-radius: 4px;
  border: 1.5px solid #35373B;
  display: flex;
  width: 415px !important;
  height: 43px;
  flex-shrink: 0;
}
input[type="text"] {
  width: 415px !important;
  height: 43px;
  flex-shrink: 0; /* You can adjust the width as needed */
}
</style>
