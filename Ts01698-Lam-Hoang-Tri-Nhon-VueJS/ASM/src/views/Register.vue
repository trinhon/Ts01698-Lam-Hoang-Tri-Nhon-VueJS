<template>
  <div class="container my-5">
    <div class="row justify-content-center">
      <div class="col-md-7">

        <div class="auth-wrapper d-flex shadow">

          <!-- KHUNG CHỮ DỌC -->
     

          <!-- FORM REGISTER -->
          <div class="auth-content flex-fill p-4">
            <h3 class="fw-bold text-center mb-4">Đăng ký</h3>

            <div class="mb-3">
              <label class="form-label">Họ tên</label>
              <input type="text" class="form-control" placeholder="Nhập họ tên" />
            </div>

            <div class="mb-3">
              <label class="form-label">Email</label>
              <input type="email" class="form-control" placeholder="Nhập email" />
            </div>

            <div class="mb-3">
              <label class="form-label">Mật khẩu</label>
              <input type="password" class="form-control" placeholder="Nhập mật khẩu" />
            </div>

            <button class="btn btn-danger w-100">
              Đăng ký
            </button>
          </div>

        </div>

      </div>
    </div>
  </div>
</template>

<style scoped>
.auth-wrapper {
  border-radius: 10px;
  overflow: hidden;
  background: #fff;
}

.auth-side span {
  writing-mode: vertical-rl;
  transform: rotate(180deg);
  color: #fff;
  font-weight: bold;
  letter-spacing: 2px;
}

.auth-content {
  background: #fff;
}
</style>
