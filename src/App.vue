<template>
  <LoginForm />
</template>
<script>
  import LoginForm from './components/LoginForm.vue'
  export default {
    data () {
      return {}
    },
    components: {
      LoginForm
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
</style>
