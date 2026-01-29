<template>
  <div class="container mt-4">
    <h2 class="mb-3">Bài 4: Quản lý bài viết</h2>

    <CreatePost @add-post="addPost" />
    <PostList :posts="posts" />
  </div>
</template>

<script setup>
import { ref } from 'vue'
import CreatePost from './components/CreatePost.vue'
import PostList from './components/PostList.vue'

const posts = ref([])

const addPost = (post) => {
  posts.value.push(post)
}
</script>
