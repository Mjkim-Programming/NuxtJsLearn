<template>
    <div class="row">
      <div class="col-md-6 mt-5 mx-auto">
        <form @submit.prevent="login" action="">
          <h2 class="h3 mb-3 font-weight-normal">로그인하기</h2>
          <div class="form-group">
            <label for="email">이메일</label>
            <input type="email" v-model="password" class="form-control" placeholder="이메일" />
          </div>
          <div class="form-group">
            <label for="password">비밀번호</label>
            <input type="password" v-model="password" class="form-control" placeholder="비밀번호" />
          </div>
          <button class="btn btn-lg btn-primary btn-block" type="submit">로그인하기</button>
        </form>
        <p class="h10 mt-3 font-weight-light">이 페이지가 마음에 드시나요?</p>
        <b-form-rating style="width:auto"></b-form-rating>
      </div>
    </div>
</template>

<script>
export default {
    name: "login",
    data:() => ({
        email: '',
        password: ''
    })
}
</script>