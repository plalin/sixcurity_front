<script>
import {useForm, Hint, validators, minLength} from "svelte-use-form";

const form=useForm();

</script>
<form use:form>

    <div class="input">
        <form class="loginBox" method="POST" action="/login_action">
          <div class="inputBox">
            <input type="text" id="id" name="id" placeholder="Enter your username" >
          </div>
          <div class="inputBox">
            <input type="password" id="id" name="pw" placeholder="Enter your password" >
          </div>
          <div class="btn">
            <button type="submit" class="loginBtn"><strong>로그인</strong></button><br>
          </div>
        </form>
        
      </div>

  </form>

  <style>

  </style>