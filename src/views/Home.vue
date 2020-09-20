<template>
  <div class="home">
    <h1 class="title is-4 mt-4 mr-4 ml-4">
      自分のブログなどの発信を<br />一つにまとめることができます。
    </h1>

    <div>
      <router-link to="/users/testJapan">
        <button class="button is-link mb-3 mt-4 is-rounded">
          TwiLinkを作成🏃
        </button>
      </router-link>
    </div>

    <div>
      <router-link to="/users/testJapan">
        <button class="button is-success mb-6 mt-4 is-rounded">
          実際のページ👀
        </button>
      </router-link>
    </div>

    <div style="display: flex; flex: flex-wrap" class="mb-4">
      <div class="column">
        <p>作成例 1</p>
        <figure class="image">
          <img src="../assets/demo.png" alt="demo" />
        </figure>
      </div>
      <div class="column">
        <p>作成例 2</p>
        <figure class="image">
          <img src="../assets/demo.png" alt="demo" />
        </figure>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Home',
  components: {}
})
</script>
