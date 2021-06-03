<template>
  <article class="w-auto h-auto bg-white">
    <img :src="image" :alt="title" class="w-64">
    <p class="py-3">
      <span class="px-2">:heart:</span>
      <span class="px-4">{{ title }}</span>
    </p>
  </article>
</template>

<script>
export default {
  name: 'Photo-Card',
  props: {
    image: {
      type: String,
      default: ''
    },
    title: {
      type: String,
      default: ''
    }
  }
}
</script>