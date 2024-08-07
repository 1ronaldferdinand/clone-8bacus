<template>
    <div class="slider" @mouseenter="stopSlider" @mouseleave="startSlider">
        <div
            class="slider-container"
            :style="{ transform: `translateX(-${currentTranslateX}%)`, transition: transitionStyle }"
        >
            <div class="slide" v-for="(image, index) in visibleImages" :key="index">
                <img :src="image" />
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
                require('@/assets/logos/image1.png'),
                require('@/assets/logos/image2.png'),
                require('@/assets/logos/image3.png'),
                require('@/assets/logos/image4.png'),
            ],
            visibleImages: [],
            currentIndex: 1, // Start from the first image (index 1)
            currentTranslateX: 100, // Position of the first image in the visibleImages
            transitionStyle: 'transform 0.5s ease',
            timer: null,
        };
    },
    created() {
        this.initSlider();
    },
    mounted() {
        this.startSlider();
    },
    beforeDestroy() {
        this.stopSlider();
    },
    methods: {
        initSlider() {
            this.visibleImages = [
                this.images[this.images.length - 1], 
                ...this.images,
                this.images[0]
            ];
        },
        startSlider() {
            this.timer = setInterval(this.nextSlide, 2000);
        },
        stopSlider() {
            clearInterval(this.timer);
        },
        nextSlide() {
            this.stopSlider();
            this.currentIndex++;
            this.currentTranslateX += 100;
    
            if (this.currentIndex > this.images.length) {
                this.resetSlider(1);
            }
            this.startSlider();
        },
        prevSlide() {
            this.stopSlider();
            this.currentIndex--;
            this.currentTranslateX -= 100;
    
            if (this.currentIndex < 1) {
                this.resetSlider(this.images.length);
            }
            this.startSlider();
        },
        resetSlider(newIndex) {
            this.transitionStyle = 'none';
            this.currentIndex = newIndex;
            this.currentTranslateX = this.currentIndex * 100;
            this.$nextTick(() => {
            this.transitionStyle = 'transform 0.5s ease';
            });
        },
    },
};
</script>
  
<style scoped>
.slider {
    position: relative;
    width: 100%;
    max-width: 600px;
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
    width: 100%;
    max-width: 480px;
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
  
@media (max-width: 992px) {
    .slide img {
        width: 100%;
    }
}
</style>
  