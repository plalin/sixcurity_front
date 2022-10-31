<!--./src/Component/Home/Home.svelte-->

<script>
import {useForm, Hint, validators, minLength} from "svelte-use-form";

const form=useForm();

</script>

<form use:form>

    <div class="input">
        <form class="loginBox" method="POST" action="/user/login">
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


    .input{
    background-color: white;
    overflow:hidden; height:auto; /*컨텐츠 추가시 자동으로 높이 크기 조절*/
    min-height: 480px;
    max-width: 450px;
    margin: 0 auto;
    border-radius: 24px;
    box-shadow: 0px 4px 23px -4px rgba(0, 0, 0, 0.25);
    text-align: center;
    align-items: center;
    justify-content: center;
    }

    .loginBox{
    padding-top: 30px;
    background-color: transparent;
    }

    .inputBox{
    width: 280px;
    margin: 0 auto;
    border-radius: 2px;
    box-sizing: border-box;
    border-bottom: 2px solid #c7c7c7;
    display: flex;
    padding-top: 10px;
    }

    .inputBox #id{
    width: 280px;
    height: 50px;
    border: none;
    outline: none;
    padding-top: 10px;
    margin-left: 10px;
    color: #000000;
    font-size: 17px;
    box-sizing: border-box;
    }
    
    .loginBtn{
    background: #0C61FE;
    border: none;
    padding: 10px 120px;
    color: #fff;
    border-radius: 10px !important;
    cursor: pointer;
    box-shadow: 4px 4px 23px -4px rgba(0, 0, 0, 0.25);
    font-size: 0.93em;
    }

    .btn{
    padding-top: 30px;
    text-align: center;
    align-items: center;
    justify-content: center;
    width: 285px;
    margin: 0 auto;
    position: relative ;
    }



  </style>