<script>
  import Main from "./pages/Main.svelte"
  import Login from "./pages/Login.svelte"
  import Signup from "./pages/Signup.svelte"
  import Router from "svelte-spa-router";

  let routes = {
    "/": Main,
    "/login": Login,
    "/signup": Signup,
    "/main": Main
  }
</script>

<div class="container">
  <div class="tabs notification is-primary">
    <ul>
      <li><a href="/#/">Main</a></li>
      <li><a href="/#/login">Login</a></li>
      <li><a href="/#/signup">Signup</a></li>
    </ul>
  </div>
  <Router {routes}/>
</div>