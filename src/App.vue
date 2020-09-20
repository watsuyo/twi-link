<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="/">
        <img src="./assets/logo.svg" alt="ロゴ" width="100" height="100" />
      </a>
    </div>
  </nav>
  <router-view class="body" />
  <div class="mt-6 mb-4">
    <a href="https://twitter.com/watsuyo_2"
      ><button class="button is-small is-rounded">
        <figure class="image is-16x16">
          <img src="./assets/send.png" alt="send" />
        </figure>
        <span class="ml-2">運営者(@watsuyo_2)に連絡</span>
      </button></a
    >
    <a
      class="twitter-share-button ml-3"
      href="https://twitter.com/intent/tweet?text=自分のブログなどの発信を一つにまとめられるサイト%20%7C%20@testJapan%20のTwilink&url=https://twilink.com&hashtags=Twilink"
      data-size="large"
    >
      <button class="button is-small is-rounded">
        <figure class="image is-16x16">
          <img src="./assets/twitter.png" alt="Twitter" />
        </figure>
        <span class="ml-2">シェア</span>
      </button></a
    >
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  setup() {
    return {}
  }
})
</script>

<style lang="scss">
@import '../node_modules/bulma/bulma.sass';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.body {
  max-width: 700px;
  width: auto;
  margin: auto;
}
</style>
