<template>
  <div class="container">
    <div class="request">
      Don't have a VJArchitecure account?
      <router-link to="/request">Request an account</router-link>
    </div>
    <div class="login">
      <img src="@/assets/LogoVALight.svg" />
      <h4>Sign into VJArcitecture</h4>
      <input type="email" placeholder="Email" />
      <input type="password" placeholder="Password" />
      <button>Sign in</button>
      <router-link to="/recover">Forgot your password?</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "SignIn",
};
</script>

<style lang="scss" scoped>
@import "@/global-styles/colors.scss";
@import "@/global-styles/typography.scss";
.container {
  display: flex;
  justify-content: center;
  align-items: center;

  min-height: 100vh;
}
.login {
  width: 400px;
  img {
    height: 100px;
  }
}
.request {
  position: absolute;
  top: 40px;
  right: 40px;

  color: rgba(255, 255, 255, 0.3);
  a {
    color: $white;
  }
}
h4 {
  @include medium-text($teal);
  margin: 0;
  text-align: center;
}
input {
  background-color: rgba(255, 255, 255, 0.2);
  border: 1px solid rgba(255, 255, 255, 0.2);
  box-sizing: border-box;
  border-radius: 4px;

  height: 60px;
  width: 100%;

  font-size: 20px;
  color: $white;
  padding-left: 20px;
  margin-top: 20px;

  &::placeholder {
    color: rgba(255, 255, 255, 0.3);
  }
}
button {
  background: $teal;
  box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.2);
  border: none;
  border-radius: 4px;

  height: 60px;
  width: 100%;

  font-size: 20px;
  color: $white;
  margin-top: 20px;
  margin-bottom: 40px;
}
a {
  line-height: 25px;
  text-decoration: none;
  color: rgba(255, 255, 255, 0.3);
  text-align: center;
  font-size: 16px;
}
</style>