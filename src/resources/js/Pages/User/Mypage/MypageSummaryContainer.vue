<script setup>
import MypageMenuPresentational from "./MypageMenuPresentational.vue";
import FavoriteStaffPresentational from "./FavoriteStaff/FavoriteStaffPresentational.vue";
import NotificationPresentational from "./Notifications/NotificationsPresentational.vue";
</script>

<template>
  <div class="mobile-layout">
    <div class="content">
      <!-- マイページメニュー -->
      <MypageMenuPresentational />
      <!-- お気に入りスタッフ -->
      <FavoriteStaffPresentational />
      <!-- 運営からのお知らせ -->
      <NotificationPresentational />
    </div>
  </div>
</template>

<style scoped>
.mobile-layout {
  font-family: "Arial", sans-serif;
  background-color: #f5f5f5;
  max-width: 375px;
  margin: 0 auto;
}

.content {
  padding: 20px;
}
</style>
