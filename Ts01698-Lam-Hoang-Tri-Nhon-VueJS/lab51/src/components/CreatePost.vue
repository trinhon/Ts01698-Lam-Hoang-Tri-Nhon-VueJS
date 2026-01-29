<template>
  <div class="card p-3 mb-4">
    <h3>Tạo bài viết mới</h3>

    <input
      v-model="post.title"
      class="form-control mb-2"
      placeholder="Tiêu đề"
    />

    <input
      v-model="post.author"
      class="form-control mb-2"
      placeholder="Tác giả"
    />

    <textarea
      v-model="post.content"
      class="form-control mb-2"
      placeholder="Nội dung"
    ></textarea>

    <button class="btn btn-primary" @click="submitPost">
      Đăng bài
    </button>
  </div>
</template>

<script setup>
import { reactive } from 'vue'

const emit = defineEmits(['add-post'])

const post = reactive({
  title: '',
  author: '',
  content: ''
})

const submitPost = () => {
  emit('add-post', { ...post })

  // reset form
  post.title = ''
  post.author = ''
  post.content = ''
}
</script>
