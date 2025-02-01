<template>
  <div class="about">
    <h1 class="about_title">About me</h1>
    <div class="profile_container">
      <img src="../assets/ringicon_0126013733.png" alt="プロフィール画像" class="profile_image" />
      <div class="profile_info">
        <p class="name">Tatsuki Ishikawa</p>
        <p class="birthday">生年月日 | 2000/06/16</p>
        <a href="https://x.com/i0ry_y" class="X_image" >
          <img src="../assets/logo-black.png" alt="x"/>
        </a>
        
      </div>
    </div>
      <div class="Skills_title">
        <h1>Skills</h1>
        <p class="skill">PHP</p>
        <p class="skill">Laravel</p>
        <p class="skill">MySQL</p>
        <p class="skill">JavaScript</p>
        <p class="skill">Vue.js</p>
        <p class="skill">JQuery</p>
        <p class="skill">TypeScript</p>
        <p class="skill">Docker</p>
        <p class="skill">AWS</p>
        <p class="skill">React</p>
      </div>
      <div class="profile">
        <h1>Profile</h1>
        <p>大阪の自社開発企業に拾っていただき現在バックエンドをメインにおまんま食べてます</p>
        <p>お酒とゲームが好きですが、飲み過ぎてしまうので最近は控えめにしてます</p>
        <p>最近はフロントエンドも勉強中です</p>
      </div>
      <div class="history">
        <h1>History</h1>
        <ul class="history_list">
          <li>
            <time class="time">2018/03</time>
            <a class="comment" href="https://cms.miyazaki-c.ed.jp/6014/">宮崎県立都城工業高校 情報学科卒業</a>
          </li>
          <li>
            <time class="time">2024/03</time>
            <a class="comment" href="https://www.sojo-u.ac.jp/">崇城大学 情報工学部卒業</a>
          </li>
          <li>
            <time class="time">2024/03</time>
            <a class="comment" href="https://www.shiftplus.co.jp/">シフトプラス株式会社 入社</a>
          </li>
        </ul>
      </div>
      <div class="portfolios">
        <h1>Portfolio</h1>
      </div>
      <div class="contactMe">
        <h1>Contact Me</h1>
        <a>
          <router-link to="/contact">Contact</router-link>
        </a>
      </div>
  </div>
</template>

<script>
export default {
  name: 'AboutView',
};
</script>

<style scoped>
.about {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
}

.skill {
  display: inline-block;
  background-color: #eeeeee;
  margin: 3px;
  padding: 3px; 
}
.about_title .Skills_title{
  font-size: 36px;
  margin-bottom: 20px;
  height: auto;
}

.profile_container {
  display: flex; /* Flexboxを使用 */
  align-items: center; /* 縦方向の中央揃え */
  justify-content: center; /* 横方向の中央揃え */
  gap: 20px; /* 画像とテキストの間隔 */
}

.profile_image {
  width: 150px; /* 画像のサイズを調整 */
  border-radius: 50%; /* 画像を円形にする */
  /* transition-delay: 80ms; /* ホバーエフェクトの遅延時間  */
}
.profile_image:hover {
  transform: scale(1.1);
  transition-delay: 70ms;
}

.profile_info {
  text-align: left; /* テキストを左揃えにする */
}

.name {
  font-size: 24px;
  margin-bottom: 5px; /* 名前と生年月日の間隔を調整 */
}

.birthday {
  font-size: 18px;
  color: #666; /* 生年月日の色を調整 */
}
.history_list{
  margin-right: 200px;
}
li {
  list-style-type: none;
}
.comment {
  color: #666;
  text-decoration: none;
  margin-left: 20%;
}
.history_list li {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.time {
  width: 100px; /* time要素の幅を固定 */
  text-align: right; /* テキストを右揃えにする */
  margin-right: 20px; /* timeとcommentの間隔を調整 */
}
.X_image img{
  width: 25px;
  height: 25px;
}
.portfolios img{
  width : 200px;
  height: 200px;
}
</style>