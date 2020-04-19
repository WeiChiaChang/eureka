<template>
  <div id="app">
    <div class="content">
      <div class="diag_line"></div>
      <div class="overlay"></div>
      <div class="name song_name eureka">ユリイカ</div>
      <div class="name song_name good_bye">グッドバ</div>
      <div class="name band_name">サ<span>カ</span>ナクション</div>
    </div>
    <!-- グッドバイ/ -->
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
  }
}
</script>

<style lang="scss">
html, body {
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Noto Serif JP', serif;
  background: black;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  .content {
    background: rgba(229, 234, 238, 1);
    width: 500px;
    height: 500px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    .name {
      color: black;
      font-size: 1.25rem;
    }
    .eureka {
      position: absolute;
      -webkit-writing-mode: vertical-lr;
      writing-mode: vertical-lr;
      letter-spacing: .6rem;
    }
    .good_bye {
      position: absolute;
      left: 31%;
      top: 48.6%;
      letter-spacing: .12rem;
    }
    .band_name {
      position: absolute;
      left: 43.9%;
      top: 54.4%;
      span {
        visibility: hidden;
      }
    }
    .diag_line {
      width: 133%;
      height: 2px;
      background: black;
      transform: rotate(135deg);
      position: absolute;
      top: 50%;
    }
    .overlay {
      position: absolute;
      background: rgba(229, 234, 238, 1);
      top: 38%;
      width: 130px;
      height: 140px;
      // border: 1px solid;
      border-radius: 50%;
    }
  }
}
</style>
