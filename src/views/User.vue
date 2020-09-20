<template>
  <div class="about">
    <figure class="image is-96x96 is-vertical-center">
      <img
        class="is-rounded"
        src="https://bulma.io/images/placeholders/128x128.png"
      />
    </figure>

    <h1 class="title mt-4">@{{ $route.params.id }}</h1>

    <div v-for="(service, index) in serviceList" :key="index" class="mt-4 mb-4">
      <a :href="service.link">
        <div class="box mr-4 ml-4">
          <article class="media">
            <div class="media-left">
              <figure class="image is-64x64">
                <img :src="service.img" :alt="service.name" />
              </figure>
            </div>
            <div class="media-content" style="height: 64px;">
              <h2 class="title is-4 mt-4 mb-4">{{ service.name }}</h2>
            </div>
          </article>
        </div>
      </a>
    </div>
  </div>
</template>

<script lang="ts">
import { reactive, computed } from 'vue'

export default {
  name: 'User',
  setup() {
    const state = reactive({
      serviceList: computed(() => [
        {
          img: 'https://bulma.io/images/placeholders/128x128.png',
          name: 'note',
          link: 'https://note.com/'
        },
        {
          img: 'https://bulma.io/images/placeholders/128x128.png',
          name: 'Qita',
          link: 'https://note.com/'
        },
        {
          img: 'https://bulma.io/images/placeholders/128x128.png',
          name: 'GitHub',
          link: 'https://note.com/'
        },
        {
          img: 'https://bulma.io/images/placeholders/128x128.png',
          name: 'はてなブログ',
          link: 'https://note.com/'
        },
        {
          img: 'https://bulma.io/images/placeholders/128x128.png',
          name: '欲しい物リスト',
          link: 'https://note.com/'
        }
      ])
    })

    return {
      serviceList: state.serviceList
    }
  }
}
</script>

<style lang="scss" scoped>
.is-vertical-center {
  margin: 0 auto;
}
</style>
