<template>
    <div>
        <div class="top-background"></div>
        <div class="my-container bg-black">
            <h2 class="service-text">Industries We Serve</h2>
            <div class="d-flex align-items-start justify-content-center" style="gap: 20px;">
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0010.png" height="80" style="margin: 0px 60px;">
                    <span>Technology</span>
                </div>
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0011.png" height="80" style="margin: 0px 60px;">
                    <span>Service Type</span>
                </div>
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0012.png" height="80" style="margin: 0px 60px;">
                    <span>Healthcare</span>
                </div>
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0013.png" height="80" style="margin: 0px 60px;">
                    <span>Banking & Infrastructure</span>
                </div>
            </div>
            <div class="d-flex align-items-start justify-content-center" style="gap: 20px;">
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0014.png" height="80" style="margin: 0px 60px;">
                    <span>Financial Technology</span>
                </div>
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0015.png" height="80" style="margin: 0px 60px;">
                    <span>Retail</span>
                </div>
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0017.png" height="80" style="margin: 0px 60px;">
                    <span>E-Commerce</span>
                </div>
                <div class="my-card">
                    <img src="@/assets/icons/8b-icon-0016.png" height="80" style="margin: 0px 60px;">
                    <span>Manufacturing & Others</span>
                </div>
            </div>
            <p style="max-width: 980px; color: white; font-size: 12px; font-family: 'Roboto', sans-serif;">
                Your concerns are our priority. 
                We proactively collaborate with you to understand your challenges and goals, 
                ensuring that our services are perfectly aligned with your vision for success. 
                We pride ourselves on being responsive and attentive partners, 
                ready to address your needs and provide timely solutions.
            </p>
        </div>
        <div class="mid-background"></div>
        <div class="my-container" style="padding: 50px 80px;">
            <span class="our-partners-text">Our Partners</span>
            <SliderImage/>
        </div>
        <div class="bot-background"></div>
    </div>
</template>

<script>
import SliderImage from '@/components/SliderImage.vue'

export default {
    components: {
        SliderImage
    }
}
</script>

<style scoped>
.our-partners-text {
    font-family: "roboto", sans-serif;
    font-size: 32px;
    line-height: 32px;
    font-weight: 600;
}

.my-card {
    border-radius: 8px;
    background-color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    gap: 20px;
    padding: 12px;
}

.my-card span{
    font-family: "Roboto", Sans-serif;
    font-size: 18px;
    line-height: 18px;
    font-weight: 600;
    color: black;
}

.my-container {
    padding: 0px 80px 100px 80px; 
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
    color:#F37721
}

.top-background {
    background-image: url('@/assets/bg/background10.png'); 
    background-size: cover; /* Adjust the background size */
    background-position: center; /* Position the background in the center */
    background-repeat: no-repeat; /* Ensure the background doesn't repeat */
    width: 100%;
    height: 300px;
    border: none;
    position: relative;
    top: 2px;
}

.mid-background {
    background-image: url('@/assets/bg/background11.png'); 
    background-size: cover; /* Adjust the background size */
    background-position: center; /* Position the background in the center */
    background-repeat: no-repeat; /* Ensure the background doesn't repeat */
    width: 100%;
    height: 300px;
    border: none;
    position: relative;
    top: -2px;
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
</style>