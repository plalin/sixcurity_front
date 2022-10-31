<!--./src/Component/Home/Home.svelte-->

<script>
    import {useForm, Hint, validators, minLength} from "svelte-use-form";
    
    const form=useForm();
    
    </script>
    
    
    <form use:form>

        <div class="input">
            <form class="joinBox" method="POST" onsubmit="return checkAll()" action="/user/join" >
                <div class="inputJBox">
                    <span class="star">*</span>
                    <input type="text" id="nickname" name="nickname" placeholder="닉네임 입력 (5 ~ 20자)" required="required" autofocus="autofocus">
                </div>
                <span class="error_next_box"></span>
                <div class="inputJBox">
                    <span class="star">*</span>
                    <input type="text" id="id" name="id" placeholder="아이디 입력 (5 ~ 20자)" required="required" autofocus="autofocus">
                </div>
                <span class="error_next_box"></span>
                <div class="inputJBox">
                    <span class="star">*</span>
                    <input type="password" id="pw" name="pw" placeholder="비밀번호 입력 (문자, 숫자, 특수문자 포함 8 ~ 16자)" required="required" autofocus="autofocus">
                </div>
                <span class="error_next_box"></span>
                <div class="inputJBox">
                    <span class="star">*</span>
                    <input type="password" id="pw_check" name="pw_check" placeholder="비밀번호 재입력" required="required" autofocus="autofocus">
                </div>
                <span class="error_next_box"></span>

                <br><br>

                <div class="btn" style="padding-top: 0;">
                    <button type="submit" class="loginBtn" style="padding: 10px 35px; border-radius:5px !important; font-size: 13px;"><strong>회원가입 완료</strong></button><br>
                </div>
            </form>
        </div>
    
    </form>
    
    <style>

    .star{
    height: 24px;
    margin: 3px 0px;
    color:red;
    border-bottom: 3px solid #c7c7c7;
    }

    .joinBox{
    padding: 50px 10px 20px 10px;
    background-color: transparent;
    }
    

    .inputJBox{
    width: 350px;
    margin: 0 auto;
    border-radius: 2px;
    box-sizing: border-box;
    display: flex;
    padding-top: 15px;
    }

    .inputJBox #id, #nickname{
    width: 350px;
    height: 30px;
    border: none;
    outline: none;
    border-bottom: 3px solid #c7c7c7;
    padding-top: 10px;
    padding-bottom: 10px;
    color: #000000;
    font-size: 12px;
    box-sizing: border-box;
    }

    .inputJBox #pw, #pw_check{
    width: 350px;
    height: 30px;
    border: none;
    outline: none;
    padding-top: 10px;
    padding-bottom: 10px;
    border-bottom: 3px solid #c7c7c7;
    color: #000000;
    font-size: 12px;
    box-sizing: border-box;
    }

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