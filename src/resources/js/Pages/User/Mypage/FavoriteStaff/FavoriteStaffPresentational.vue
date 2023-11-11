<template>
  <div class="user-profiles">
    <div class="user">
      <img src="/images/user.jpg" alt="ユーザー" />
      <span>ユーザーname</span><br />
      <span class="shop-name">ショップname</span>
    </div>
    <div class="user">
      <img src="/images/user.jpg" alt="ユーザー" />
      <span>ユーザーname</span><br />
      <span class="shop-name">ショップname</span>
    </div>
    <div class="user">
      <img src="/images/user.jpg" alt="ユーザー" />
      <span>ユーザーname</span><br />
      <span class="shop-name">ショップname</span>
    </div>
  </div>
</template>

<style scoped>
.user-profiles {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
  margin-top: 20px;
}

.user {
  text-align: center;
  font-size: 0.8em;
}

.shop-name {
  color: gray;
}

.user img {
  width: 80px;
  height: 80px;
  border-radius: 20%;
  margin-bottom: 5px;
}
</style>