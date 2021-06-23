<template>
  <div class="login-form">
    <form>
      <fieldset>
        <legend>Login</legend>
        <div>
          <label for="email">email address</label>
          <input id="email" type="text" required>
        </div>
        <div>
          <label for="password">password</label>
          <input id="password" type="password" required>
        </div>
        <button>Login</button>
      </fieldset>
    </form>
  </div>
</template>
<script>
  export default {
    data () {
      return {}
    }
  }
</script>
<style>
body {
  margin: 0;
  height: calc(100vh);
  background-color: #F4F5F7;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: "Helvetica Neue",Helvetica,Arial,sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.login-form {
  background-color: #FFFFFF;
  border: none;
}
form {
  padding: 1em;
  width: 350px;
}
fieldset {
  margin: 0;
  border: none;
}
fieldset legend {
  margin-bottom: 1rem;
  font-weight: bold;
  font-size: 1.8em;
}
fieldset label {
  color: #6E7381;
  text-transform: uppercase;
  font-weight: bold;
  font-size: 12px;
  letter-spacing: .1rem;
}
fieldset > div {
  display: flex;
  flex-direction: column;
  margin-bottom: 2em;
}
fieldset > div input {
  margin-top: 1em;
  padding: 1em;
  font-size: 1em;
  border: 1px solid #E5E7EB;
}
button {
  width: 100%;
  border: none;
  color: #FFFFFF;
  background-color: #217BC7;
  border-radius: 26px;
  font-size: 1em;
}
</style>
