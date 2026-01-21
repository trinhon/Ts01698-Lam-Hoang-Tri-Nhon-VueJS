<template>
<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container">
    <a class="navbar-brand" href="#">ASM</a>

    <div class="collapse navbar-collapse">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item">
          <router-link class="nav-link" to="/">Home</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/posts">Bài viết</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/login">Đăng nhập</router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/register">Đăng ký</router-link>
        </li>
      </ul>
    </div>
  </div>
</nav>
</template>
