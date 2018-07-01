<template>
	<div class="container">
	<div class="row">
	<div class="col-sm-8">
		<div class="block_line" style="padding-top:5px;padding-left:8px;padding-bottom:10px;">
			<font color="blue"><b>自我介紹</b></font>
		<div class="row">
          <div class="col-sm-9">
             <textarea  id="user_dsp" name="user_dsp" rows="6" style="width:100%;">Hi, I am little doge.&#10;測試中...</textarea>
          </div>
          <div class="col-sm-3">
            2017-06-20 加入<br>
            現居苗栗市<br>
            就讀苗栗國中一年級<br>
            以連結至 facebook 帳戶
          </div>
		</div>
		</div>
		<br>
	<div class="row">
		<div class="col-sm-6">
			<div class="block_line" style="padding-top:5px;padding-left:8px;padding-bottom:10px;">
			<font color="blue"><b>我的學習紀錄</b></font><br>
			發問次數: {{answer_number}} <br>
			回答次數: 1 <br>
			白板參與次數: 5 <br>
			最佳解答次數: 1 <br>
			英語話劇參與次數: 0 <br>
			題庫挑戰次數: 3 <br>
			競賽參與次數: 2 <br>
			創建筆記次數: 11 <br>
			收藏筆記次數: 23 <br>
			收藏問題數: 56 <br>
			<br>
			</div>
		</div>
		<div class="col-sm-6">
			<div class="block_line" style="padding-top:5px;padding-left:8px;padding-bottom:10px;">
			<font color="blue"><b>我的學習歷程</b></font><br>
			用戶組: 國一 <br>
			積分: 593 <br>
			好友數: 5 <br>
			登入次數: 120 <br>
			在線時間: 227小時 <br>
			完成任務: 0 <br>
			</div>
			<div class="block_line" style="padding-top:5px;padding-left:8px;padding-bottom:10px;">
			<font color="blue"><b>勳章 成就 頭銜</b></font><br>
			<br>
			努力中.. 目前尚無 <br>
			<br>
			</div>
		</div>

    </div>
	</div>

	<div class="col-sm-2">
    <div class="block_line" style="padding-top:5px;padding-left:3px;padding-bottom:5px;min-height:185px;">
      <font color="blue"><b>好友推薦-同校的學生</b></font><br>

	  <table style="padding:10px;">
	  <tr><td height="35">
	  <a class="btn btn-primary btn-sm" data-toggle="modal" data-target="#user_1">hua98:小華</a></td></tr>
	  <tr><td>
	  <a class="btn btn-primary btn-sm" data-toggle="modal" data-target="#user_2">rick:小馬</a></td></tr>
      </table>


      <br>
    </div>
    <br>
    <div class="block_line" style="padding-top:5px;padding-left:3px;padding-bottom:5px;min-height:185px;">
      <font color="blue"><b>好友推薦-同縣市的學生</b></font><br>

	  <table style="padding:10px;">
	  <tr><td height="35">
	  <a class="btn btn-primary btn-sm" data-toggle="modal" data-target="#user_1">skyfly: 蓉蓉</a></td></tr>
	  <tr><td>
	  <a class="btn btn-primary btn-sm" data-toggle="modal" data-target="#user_2">aizhen93: 艾珍</a></td></tr>
      </table>

      <br>
    </div>
	</div>

	</div>
	</div>
</template>

<script>
	export default {
		data(){
			return{
				answer_number :15,
			}
		}
	}
</script>

<style lang="css">
</style>
