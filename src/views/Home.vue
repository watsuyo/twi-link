<template>
  <div class="home">
    <router-link to="/users/testJapan">
      <button class="button is-primary">TwiLinkを作成</button>
    </router-link>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Home',
  components: {}
})
</script>
