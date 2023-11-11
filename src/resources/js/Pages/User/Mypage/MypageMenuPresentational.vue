<template>
  <div class="rewards-section">
    <div class="icon-box">
      <img src="/images/icons/point.jpg" alt="ポイント" />
      <span>ポイント<br />100,000CP</span>
    </div>
    <div class="icon-box">
      <img src="/images/icons/profile.jpg" alt="プロフィール" />
      <span>プロフィール</span>
    </div>
    <div class="icon-box">
      <img src="/images/icons/megahon.jpg" alt="応援履歴" />
      <span>応援履歴</span>
    </div>
    <div class="icon-box">
      <img src="/images/icons/ranking.jpg" alt="ランキング" />
      <span>ランキング</span>
    </div>
    <button class="reward-button">ショップ一覧</button>
    <button class="reward-button">ポイントチャージ</button>
  </div>
</template>

<style scoped>
.rewards-section {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 10px;
  background-color: #fff;
  padding: 20px;
  border-radius: 8px;
  align-items: center;
}

.coin-box,
.icon-box {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 10px;
  background-color: #f6f6f6;
  border-radius: 8px;
}

.icon-box img {
  width: 30px;
  height: 30px;
}

.reward-button {
  grid-column: span 2;
  padding: 10px;
  background-color: #ffd700;
  border: none;
  border-radius: 8px;
  font-weight: bold;
  color: #fff;
  cursor: pointer;
  margin-top: 10px;
}

.reward-button:hover {
  background-color: #ffc700;
}
</style>