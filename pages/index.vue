<template>
  <div class="container">
  
  <header class="header__inner">
    <h3>
      取引  <input type='text'> <button @click="search">検索</button>
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

    <div>
      <h3 class="subheader__inner">
        <button @click="pipeline" class="button--grey">パイプライン</button> <button @click="list" class="button--grey">リスト</button> <button @click="add" class="button--green">追加</button>
      </h3>
      <div class="wrapper">
        <main class="main__topic">
          返信済み/見積もり中
        </main>
        <main class="main__topic">
          見積もり送付済み
        </main>
        <main class="main__topic">
        受注確定/請求書発行
        </main>
        <main class="main__topic">
          請求書発行済/制作指示済
        </main>
        <main class="main__topic">
          検収中/追加の請求書発行
        </main>
      </div>
      <div class="wrapper">
        <main class="main">
          コンテンツ
        </main>
        <main class="main">
          コンテンツ
        </main>
        <main class="main">
          コンテンツ
        </main>
        <main class="main">
          コンテンツ
        </main>
        <main class="main">
          コンテンツ
        </main>
      </div>
    </div>
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

.header__inner {
  position: relative;
  height: 10vh;
  border: 1px solid #1cd688;
  background-color: #e7ffe8;
}

.wrapper {
  display: flex;
  max-width: relative;
  margin: 2.5em auto;
}

.subheader__inner {
  position: relative;
  height: 5vh;
  border: 1px solid #d6336c;
  background-color: #fff0f6;
}

.sidebar {
  width: 10%;
  margin-right: 1em;
}


.sidebar__inner {
  position: relative;
  height: 150vh;
  border: 1px solid #1c7ed6;
  background-color: #e7f5ff;
}

.main__topic {
  display: flex;
  position: relative;
  width: 20%;
  height: 5vh;
  border: 1px solid #d6336c;
  background-color: #fff0f6;
}

.main {
  position: relative;
  width: 20%;
  height: 300vh;
  border: 1px solid #d6336c;
  background-color: #fff0f6;
}


</style>
