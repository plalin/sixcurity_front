<!--./src/Component/Header/Header.svelte-->
<nav>
  <a href="#/">Home</a>
  <a href="#/Contact1">Contact1</a>
  <!-- App컴포넌트에서 '/Contact2/:test' 여기의 :test
  		가 1234가 된다.-->
  <a href="#/Contact2/1234">Contact2</a>
  <a href="#/Login">Login</a>
  <a href="#/SignIn">SignIn</a>
  <br><br><br><br>
</nav>



<style>
  a {
    text-decoration: none !important;
  }
</style>