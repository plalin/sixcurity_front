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
                                </tr>
                            </thead>
                            <tbody id="mytable">

                            </tbody>
                        </table>
                    </div>
                <a class="test_manage_btn" href="/Group">서비스 추가하기</a>
                
        </div>

    </div>


</form>