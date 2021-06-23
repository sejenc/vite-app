<template>
  <div>
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
