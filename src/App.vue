<template>
<div>
  <Login />
</div>
</template>

<script>
import Header from './components/Header';
import Main from './components/Main';
import Bottom from './components/Bottom';
import Footer from './components/Footer';
import Register from './pages/Register';
import Login from './pages/Login';


export default {
  name: 'App',

  components: {
    Header,
    Main,
    Footer,
    Bottom,
    Register,
    Register,
    Login
  }
}
</script>

<style lang="scss">

</style>