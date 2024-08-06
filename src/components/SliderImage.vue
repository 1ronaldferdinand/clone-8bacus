<template>
    <div class="slider">
        <div class="slider-container" :style="{ transform: `translateX(-${currentIndex * 100}%)` }">
            <div class="slide">
                <img src="@/assets/logos/image1.png">
            </div>
            <div class="slide">
                <img src="@/assets/logos/image2.png">
            </div>
            <div class="slide">
                <img src="@/assets/logos/image3.png">
            </div>
            <div class="slide">
                <img src="@/assets/logos/image4.png">
            </div>
        </div>
        <button class="prev chevron" @click="prevSlide">&#10094;</button>
        <button class="next chevron" @click="nextSlide">&#10095;</button>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            images: [
                '@/assets/logos/image1.png',
                '@/assets/logos/image2.png',
                '@/assets/logos/image3.png',
                '@/assets/logos/image4.png'
            ],
            currentIndex: 0,
            timer: null
        };
    },
    mounted() {
        this.startSlider();
    },
    beforeDestroy() {
        this.stopSlider();
    },
    methods: {
        startSlider() {
            this.timer = setInterval(this.nextSlide, 2000);
        },
        stopSlider() {
            clearInterval(this.timer);
        },
        prevSlide() {
            this.stopSlider();
            this.currentIndex = (this.currentIndex + this.images.length - 1) % this.images.length;
            this.startSlider();
        },
        nextSlide() {
            this.stopSlider();
            this.currentIndex = (this.currentIndex + 1) % this.images.length;
            this.startSlider();
        }
    }
};
</script>
  
<style scoped>
    .slider {
        position: relative;
        width: 600px;
        overflow: hidden;
    }
  
    .slider-container {
        display: flex;
        transition: transform 0.5s ease;
    }
  
    .slide {
        min-width: 100%;
        box-sizing: border-box;
        display: flex;
        justify-content: center;
        align-items: center;
    }
  
    .slide img {
        width: 480px;
        display: block;
    }
  
    button {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        background-color: rgba(0, 0, 0, 0.5);
        border: none;
        color: white;
        font-size: 24px;
        padding: 10px;
        cursor: pointer;
    }
  
    .prev {
        left: 10px;
    }
  
    .next {
        right: 10px;
    }

    .chevron {
        background: none;
        color: #F47721;
    }
</style>
  