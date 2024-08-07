<template>
    <div>
        <div class="top-background"></div>
        <div class="my-container bg-black">
            <div class="d-flex align-items-center justify-content-center gap-3">
                <h2 class="service-text m-0 text-white">Connect With</h2>
                <img class="our-logo" src="@/assets/cropped-top-logo-head.png" height="54">
            </div>
            <p>We are your dedicated partner on the path to success.</p>
            <div class="map-container">
                <iframe
                    src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d1930.8562713776294!2d121.019265!3d14.558424!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3397c94ae4f2887d%3A0x4f8768415d368f09!2sPBCom%20Tower!5e0!3m2!1sen!2sid!4v1722946084901!5m2!1sen!2sid"
                    class="responsive-iframe"
                    allowfullscreen=""
                    loading="lazy"
                    referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style scoped>
p {
    font-family: "roboto", sans-serif;
    font-size: 12px;
    line-height: 14px;
    font-weight: 400;
    color: white;
}

.my-container {
    padding: 0px 80px 30px 80px; 
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    border: none;
    gap: 20px;
}

.service-text {
    font-family: "Roboto", Sans-serif;
    font-size: 34px;
    font-weight: 600;
    line-height: 40px;
}

.top-background {
    background-image: url('@/assets/bg/background10.png'); 
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    width: 100%;
    height: 300px;
    border: none;
    position: relative;
    top: 2px;
}

.map-container {
    position: relative;
    width: 100%;
    padding-top: 56.25%; /* 16:9 Aspect Ratio */
}

.responsive-iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
}

@media (max-width: 992px) {
    .my-container {
        padding: 0px 40px 30px 40px;
        gap: 10px;
    }

    .service-text {
        font-size: 20px;
    }

    .our-logo {
        height: 30px !important;
    }
}
</style>
