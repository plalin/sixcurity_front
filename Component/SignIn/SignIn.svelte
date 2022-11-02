<script>
    import {useForm, Hint, validators, minLength} from "svelte-use-form";
    const form=useForm();
</script>
    
    
<form use:form>
    <div class="input">
        <form class="joinBox" method="POST" onsubmit="return checkAll()" action="/SignIn_action" >
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