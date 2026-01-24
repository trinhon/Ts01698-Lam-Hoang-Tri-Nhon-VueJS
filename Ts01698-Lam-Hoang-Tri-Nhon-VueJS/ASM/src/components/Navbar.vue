<template>
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <router-link to="/" class="navbar-brand">Báo Giải Trí</router-link>

    <ul class="navbar-nav ms-auto">
      <li class="nav-item">
        <router-link class="nav-link" to="/">Trang chủ</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/posts">Bài viết</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/posts/create">Thêm bài viết</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/login">Đăng nhập</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/register">Đăng ký</router-link>
      </li>
    </ul>
  </div>
</nav>
</template>
