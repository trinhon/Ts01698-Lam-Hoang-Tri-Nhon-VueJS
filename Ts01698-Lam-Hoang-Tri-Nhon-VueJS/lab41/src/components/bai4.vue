<template>
    <div class="container mt-5">
        <h1 class="text-center">Chill</h1>
        <div class="row">
            <div class="col-sm-4">
                <div class="card">
                    <img :src="items[0].image" alt="Hình ảnh" />
                    <div class="card-body">
                        <h3 class="card-title">{{ items[0].title }}</h3>
                        <p class="card-text">{{ items[0].content }}</p>
                        <button class="btn btn-info">Xem chi tiết </button>
                    </div>
                </div>
            </div>
            <div class="col-sm-4">
                <div class="card">
                    <img :src="items[1].image" alt="Hình ảnh" />
                    <div class="card-body">
                        <h3 class="card-title">{{ items[1].title }}</h3>
                        <p class="card-text">{{ items[1].content }}</p>
                        <button class="btn btn-info">Xem chi tiết </button>
                    </div>
                </div>
            </div>
            <div class="col-sm-4">
                <div class="card">
                    <img :src="items[2].image" alt="Hình ảnh" />
                    <div class="card-body">
                        <h3 class="card-title">{{ items[2].title }}</h3>
                        <p class="card-text">{{ items[2].content }}</p>
                        <button class="btn btn-info">Xem chi tiết </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
// Import hình ảnh từ thư mục assets
import img1 from '../assets/images/nhan.png';
import img2 from '../assets/images/nhan2.jpg';
import img3 from '../assets/images/nhan3.jpg';

const items = ([
    {
        title: 'ha nhan', 
        content: '...', 
        image: img1
    },
    {
        title: 'ha nhan 2', 
        content: '...',
        image: img2
    },
    {
        title: 'ha nhan 3', 
        content: '...', 
        image: img3
    },
]);
</script>