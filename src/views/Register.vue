<template>
<div class="container">
  <form @submit.prevent="onAuthSubmit" class="form-horizontal">
    <div class="form-group">
      <label class="control-label col-sm-2">使用者暱稱:</label>
      <div class="col-sm-10 form-inline">
        <input type="text" class="form-control" style="width:203px" name="nick_name" v-model="nick_name">
        <button type="submit" class="btn btn-default">檢查重複</button>
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">自我介紹:</label>
      <div class="col-sm-10">
        <textarea class="form-control" style="width:286px" name="nick_name" rows="6" v-model="introduce_txt"></textarea>
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">電子郵件:</label>
      <div class="col-sm-10">
        <input type="email" class="form-control" style="width:286px" aria-describedby="emailhelp" name="user_id" v-model="user_id">
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">居住地:</label>
      <div class="col-sm-10">
        <input type="text" class="form-control" style="width:203px" name="user_city" v-model="user_city">
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">出生年月日:</label>
      <div class="col-sm-10">
        <input type="date" class="form-control" style="width:203px" name="user_birth" v-model="user_birth">
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">手機號碼:</label>
      <div class="col-sm-10 form-inline">
        <input type="tel" class="form-control" style="width:203px" name="user_mobile" v-model="user_mobile">
        <input type="checkbox" class="form-check-input" />我沒有手機
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">帳戶綁定:</label>
      <div class="col-sm-10 form-inline">
        <button type="submit" class="btn btn-default">Facebook</button>
        <button type="submit" class="btn btn-default">Google+</button>
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">目前就讀學校:</label>
      <div class="col-sm-10 form-inline">
        <input type="text" class="form-control" style="width:203px" name="school" v-model="school">
        <input type="checkbox" name="grade_cd" />我已經畢業
      </div>
    </div>

    <div class="form-group">
      <label class="control-label col-sm-2">年級:</label>
      <div class="col-sm-10 form-inline">
        <input type="text" class="form-control" style="width:203px" name="school_grade" v-model="school_grade">
      </div>
    </div>


    <div class="form-group">
      <label class="control-label col-sm-2">設定密碼:</label>
      <div class="col-sm-10">
        <input type="password" class="form-control" style="width:203px" placeholder="請輸入密碼" name="user_pwd" v-model="user_pwd">
      </div>
    </div>
    <div class="form-group">
      <label class="control-label col-sm-2">確認密碼:</label>
      <div class="col-sm-10 form-inline">
        <input type="password" class="form-control" placeholder="請再輸入一次密碼" name="user_pwd2" v-model="user_pwd2">
      </div>
    </div>
    <div class="form-group">
      <div class="col-sm-offset-2 col-sm-10">
        <button type="submit" class="btn btn-default">Submit</button>
      </div>
    </div>
  </form>
  {{status}}

</div>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      password: "",
      status: null
    }
  },
  method: {
    onAuthSubmit() {
      console,
      log(this.email, this.password)
      if (this.email == "aaa@gmail.com" && this.password == "123") {
        this.status = "登入成功"
      } else {
        this.status = "登入失敗"
      }
    }
  }
}
</script>

<style lang="css">
</style>
