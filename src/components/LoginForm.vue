<template>
  <div class="login-form">
    <form @submit.prevent="onSubmit">
      <fieldset>
        <legend>Login</legend>
        <div>
          <label for="email">email address</label>
          <input 
            v-model="email" 
            id="email" 
            type="text" 
            required
          >
        </div>
        <div>
          <label for="password">password</label>
          <input 
            v-model="password" 
            id="password" 
            type="password"
            minlength="6" 
            required
          >
        </div>
        <button
          type="submit" 
          :disabled="!isEmailValid"
        >
          Login
        </button>
      </fieldset>
    </form>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        email: '',
        password: ''
      }
    },
    methods: {
      onSubmit () {
        alert('Login successful!')
        this.resetForm()
      },
      resetForm () {
        this.email = ''
        this.password = ''
      }
    },
    computed: {
      isEmailValid () {
        return /^([a-z]){1,}@([a-z]){1,}.com/.test(this.email)
      }
    }
  }
</script>
<style>
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
  padding: 1em;
  border: none;
  color: #FFFFFF;
  background-color: #217BC7;
  border-radius: 26px;
  font-size: 1em;
}
</style>