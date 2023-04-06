<template>
  <SignIn />
  <SignUp />
  <AppointmentPage />
</template>

<script>

//import SignIn from './components/SignIn.vue';
//import SignUp from './components/SignUp.vue';
import AppointmentPage from './components/AppointmentPage';
export default {
  name: 'App',
  components:{
    //SignIn,
    //SignUp,
    AppointmentPage,
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
