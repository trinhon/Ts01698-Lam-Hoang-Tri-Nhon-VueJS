<template>
  <div>
    <div
      v-for="(post, index) in posts"
      :key="index"
      class="card p-3 mb-3"
      :class="{
        'bg-light': index % 2 === 0,
        'bg-warning': index % 2 !== 0
      }"
      :style="{
        borderLeft: '6px solid #000'
      }"
    >
      <h4>{{ post.title }}</h4>
      <p><i>Tác giả:</i> {{ post.author }}</p>
      <p>{{ post.content }}</p>
    </div>
  </div>
</template>

<script setup>
defineProps({
  posts: {
    type: Array,
    default: () => []
  }
})
</script>
