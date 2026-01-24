<template>
  <div class="col-md-8 mx-auto">
    <h3 class="mb-3">Thêm bài viết</h3>

    <div class="mb-3">
      <label class="form-label">Tiêu đề</label>
      <input
        v-model="title"
        class="form-control"
        placeholder="Nhập tiêu đề"
      />
    </div>

    <div class="mb-3">
      <label class="form-label">Nội dung</label>
      <textarea
        v-model="content"
        class="form-control"
        rows="5"
        placeholder="Nhập nội dung"
      ></textarea>
    </div>

    <button class="btn btn-primary" @click="savePost">
      Lưu bài viết
    </button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const title = ref('')
const content = ref('')

const savePost = () => {
  if (!title.value || !content.value) {
    alert('Vui lòng nhập đầy đủ thông tin')
    return
  }

  alert('Lưu bài viết thành công (demo UI)')
  title.value = ''
  content.value = ''
}
</script>
