<template>
  <div class="bg-gray-50 dark:bg-gray-800 w-full h-full flex justify-center">
    <card
      :content="content"
      @light-mode="changeModeLight"
      @dark-mode="changeModeDark"
    ></card>
  </div>
</template>
<script>
import Card from '~/components/Card.vue'
export default {
  components: { Card },
  async asyncData({ $content }) {
    const content = await $content('cardContent').fetch()
    return {
      content,
    }
  },
  methods: {
    changeModeLight() {
      localStorage.removeItem('theme')
      document.querySelector('html').classList.remove('dark')
    },
    changeModeDark() {
      localStorage.theme = 'dark'
      document.querySelector('html').classList.add('dark')
    },
  },
}
</script>
