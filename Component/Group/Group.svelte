<script>
    import {useForm, Hint, validators, minLength} from "svelte-use-form";
    const form=useForm();
</script>
    

<div class="city_edit"> 
    <h1>자산 관리</h1>
    <p>속한 그룹과 잔고를 확인할 수 있습니다.</p>
</div>

<br><br>

<div class="justBox">

    <form use:form>

        <div class="input" style="width: 500px; height:300px; margin-right:50px">
            <form class="loginBox" method="POST" action="/group_deposit">
              <div class="inputBox">
                <input type="text" id="id" name="group_deposit_id" placeholder="Enter your group id" >
              </div>
              <div class="inputBox">
                <input type="password" id="id" name="groupd_deposit_amount" placeholder="Enter amount" >
              </div>
              <div class="btn">
                <button type="submit" class="loginBtn"><strong>Deposit</strong></button><br>
              </div>
            </form>
            
          </div>
      </form>
    
      <form use:form>
    
        <div class="input" style="width: 500px; height:300px; margin-left:50px" >
            <form class="loginBox" method="POST" action="/group_withdraw">
              <div class="inputBox">
                <input type="text" id="id" name="group_withdraw_id" placeholder="Enter your group id" >
              </div>
              <div class="inputBox">
                <input type="password" id="id" name="group_withdraw_amount" placeholder="Enter amount" >
              </div>
              <div class="btn">
                <button type="submit" class="loginBtn"><strong>Withdraw</strong></button><br>
              </div>
            </form>
            
          </div>
      </form>
</div>

<br><br><br><br>

<div class="city_edit"> 
    <h1>그룹 및 유저 관리</h1>
    <p>그룹에 유저를 추가하거나 밴때리세요.</p>
</div>

<br><br>

<div class="justBox">
    <form use:form>

        <div class="input" style="width: 500px; height:300px; margin-right:50px">
            <form class="loginBox" method="POST" action="/group_invite">
              <div class="inputBox">
                <input type="text" id="id" name="group_invite_user" placeholder="Enter your user id" >
              </div>
              <div class="inputBox">
                <input type="password" id="id" name="groupd_invite_id" placeholder="Enter your group id" >
              </div>
              <div class="btn">
                <button type="submit" class="loginBtn"><strong>Invite User</strong></button><br>
              </div>
            </form>
            
          </div>
      </form>
    
      <form use:form>
    
        <div class="input" style="width: 500px; height:300px; margin-left:50px" >
            <form class="loginBox" method="POST" action="/group_ban">
              <div class="inputBox">
                <input type="text" id="id" name="group_ban_user" placeholder="Enter ban user id" >
              </div>
              <div class="inputBox">
                <input type="password" id="id" name="group_ban_id" placeholder="Enter your group id" >
              </div>
              <div class="btn">
                <button type="submit" class="loginBtn"><strong>Ban User</strong></button><br>
              </div>
            </form>
            
          </div>
      </form>
</div>
