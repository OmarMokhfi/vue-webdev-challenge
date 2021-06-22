<template>
  <div class="bg-gray-50 w-full h-full flex justify-center">
    <card :content="content"></card>
  </div>
</template>
<script>
export default {
  async asyncData({ $content }) {
    const content = await $content('cardContent').fetch()

    return {
      content,
    }
  },
}
</script>
