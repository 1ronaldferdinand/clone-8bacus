<template>
    <div>
        <div class="my-container">
            <h2 class="service-text">Company Events</h2>
            <div class="gallery-container">
                <div class="row" v-for="(row, rowIndex) in displayedImages" :key="rowIndex">
                    <div class="row p-0 d-lg-none" v-for="(image, colIndex) in row" :key="colIndex">
                        <img :src="image" alt="Gallery Image" class="gallery-image" />
                    </div>
                    <div class="column d-none d-lg-flex" v-for="(image, colIndex) in row" :key="colIndex">
                        <img :src="image" alt="Gallery Image" class="gallery-image" />
                    </div>
                </div>
            </div>
            <b-button pill @click="toggleRow" class="toggle-button">
                {{ buttonText }}
            </b-button>
        </div>
        <div class="bot-background"></div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            images: [
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
            ],
            displayedImages: [],
            rowsToShow: 2,
            showMore: false,
        };
    },
    computed: {
        buttonText() {
            return this.showMore ? 'Hide Images' : 'Show More Images';
        }
    },
    mounted() {
        this.initializeGallery();
    },
    methods: {
        initializeGallery() {
            this.displayedImages = this.chunkArray(this.images.slice(0, this.rowsToShow * 3), 3);
        },
        chunkArray(array, chunkSize) {
            let results = [];
            for (let i = 0; i < array.length; i += chunkSize) {
                results.push(array.slice(i, i + chunkSize));
            }
            return results;
        },
        toggleRow() {
            if (this.showMore) {
                this.displayedImages.pop();
            } else {
                const currentLength = this.displayedImages.length * 3;
                const newImages = this.images.slice(currentLength, currentLength + 3);
                if (newImages.length > 0) {
                    this.displayedImages.push(newImages);
                }
            }
            this.showMore = !this.showMore;
        },
    },
};
</script>

<style scoped>
.gallery-container {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.row {
    display: flex;
    justify-content: center;
}
.column {
    padding: 5px;
    margin: 5px; /* Adjusted margin for better spacing */
    width: fit-content;
}
.gallery-image {
    width: 262px;
    height: 161px;
    object-fit: cover;
    opacity: 0;
    animation: fadeIn 1s forwards;
}
.toggle-button {
    margin-top: 20px;
    padding: 10px 20px;
    background-color: #f37721;
    color: white;
    border: none;
    cursor: pointer;
}
.toggle-button:hover {
    background-color: #f47721;
}
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(-20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.my-container {
    padding: 100px 80px 50px 80px; 
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    border: none;
    gap: 20px;
}

.service-text {
    font-family: "Roboto", Sans-serif;
    font-size: 48px;
    font-weight: 600;
    color: black;
}

.bot-background {
    background-image: url('@/assets/bg/background5.png'); 
    background-size: cover; /* Adjust the background size */
    background-position: center; /* Position the background in the center */
    background-repeat: no-repeat; /* Ensure the background doesn't repeat */
    width: 100%;
    height: 300px;
    border: none;
}

@media (max-width: 992px) {
    .service-text {
        font-size: 32px;
    }

    .my-container {
        padding: 100px 40px 0px 40px;
    }

    .row {
        margin: 0px !important;
    }

    .gallery-image {
        height: auto;
        width: 100%;
        padding: 10px;
    }
}
</style>