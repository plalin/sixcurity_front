<script>
    import {useForm, Hint, validators, minLength} from "svelte-use-form";
    const form=useForm();
</script>
    
    
<form use:form>
    <div class="main_pic_bg">
        <div class="city_edit"> 
            <h1>자산 관리</h1>
            <p>속한 그룹과 잔고를 확인할 수 있습니다.</p>
            <div class="mypage_box">
                    <div class="mypage_title">
                        <div class="reg_svc_list_title">
                            현재 속한 그룹
                        </div>
                    </div>
                    <div class="table_box">
                        <table class="data_table">
                            <thead>
                                <tr>
                                    <th>번호</th>
                                    <th>그룹명</th>
                                    <th>소속 인원수</th>
                                    <th>잔고</th>
                                    <th>삭제</th>
                                </tr>
                            </thead>
                            <tbody id="mytable">

                            </tbody>
                        </table>
                    </div>
                <a class="test_manage_btn" href="/Group">그룹 관리</a>
                
        </div>
    </div>
</form>

<!--

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

-->