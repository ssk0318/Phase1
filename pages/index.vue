<template>
  <div class="container">
  
  <header class="header__inner">
    <h3>
      取引  <input type='text'> <button @click="search">検索</button>
    </h3>
    <h3>
      <!-- ↓　""コンポーネント内容変更必要　-->
      <button @click="pipeline" class="button--grey">パイプライン</button> <button @click="list" class="button--grey">リスト</button> <button @click="add" class="button--green">追加</button>
    </h3>
  </header>

  <div class="wrapper">
  <aside class="sidebar">
    <div class="sidebar__inner">
      <div>ホーム</div>
      <div>リード</div>
      <div>アクティビティ</div>
      <div>連絡先</div>
      <div>分析</div>
      <div>プロダクト</div>
    </div>
  </aside>
  
  <main class="main">
    返信済み/見積もり中
  </main>
  <main class="main">
    見積もり送付済み
  </main>
  <main class="main">
    受注確定/請求書発行
  </main>
  <main class="main">
    請求書発行済/制作指示済
  </main>
  <main class="main">
    検収中/追加の請求書発行
  </main>
  </div>

</div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
.container {
  min-height: 100vh;
  padding: 16px;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}
.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.header__inner {
  position: relative;
  height: 10vh;
  border: 1px solid #1cd688;
  background-color: #e7ffe8;
}

.wrapper {
  display: flex;
  max-width: 700px;
  margin: 2.5em auto;
}

.sidebar {
  width: 30%;
  margin-right: 1em;
}


.sidebar__inner {
  position: relative;
  height: 150vh;
  border: 1px solid #1c7ed6;
  background-color: #e7f5ff;
}

.main {
  position: relative;
  height: 300vh;
  border: 1px solid #d6336c;
  background-color: #fff0f6;
}


</style>
