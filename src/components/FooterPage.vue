<template>
    <div class="d-flex flex-column align-items-center">
        <div class="my-container d-flex flex-column flex-lg-row align-items-center align-items-lg-start justify-content-between w-100" style="padding: 64px 100px;">
            <div class="d-flex flex-column align-items-center col-12 col-lg-4" style="gap: 10px;">
                <div class="d-flex flex-column align-items-center align-items-lg-start identity-container" style="width: fit-content;">
                    <img class="our-logo" src="@/assets/cropped-top-logo-head.png" height="40" width="150">
                    <span class="light-text">
                        We go beyond services; we provide<br> solutions that empower your business to<br> thrive.
                    </span>
                    <div class="d-flex flex-column">
                        <span class="hard-text">Company landline number:</span>
                        <span class="light-text">02-53104708</span>
                    </div>
                </div>
            </div>
            <div class="col-12 col-lg-3 d-flex flex-column">
                <span class="hard-text" style="font-size: 16px; padding-bottom: 10px;">Our Services</span>
                <div class="light-text">
                    Recruitment<br>
                    Payroll Service<br>
                    Administrative Support<br>
                    Immigration / Visa Processing<br>
                    Business Registration<br>
                    Accounting & Taxation<br>
                    Business Consultancy<br>
                </div>
            </div>
            <div class="col-12 col-lg-3 d-flex flex-column">
                <span class="hard-text" style="font-size: 16px; padding-bottom: 10px;">Legal</span>
                <div class="light-text">
                    Privacy Policy<br>
                    Terms and Conditions<br>
                </div>
            </div>
            <div class="col-12 col-lg-2 d-flex flex-row flex-lg-column align-items-center justify-content-center justify-content-lg-start gap-2">
                <img src="@/assets/icons/fb.png" height="20" width="20">
                <img src="@/assets/icons/insta.png" height="20" width="20">
                <img src="@/assets/icons/linkedin.png" height="20" width="20">
                <img src="@/assets/icons/tiktok.png" height="20" width="20">
            </div>
        </div>
        <div class="credit-section">
            <span class="roboto-text">©8Bacus Corporation 2024, All rights reserved.</span>
        </div>
        <div class="bg-black w-100" style="height: 30px;"></div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.roboto-text {
    font-family: "Roboto", sans-serif;
}

.hard-text {
    font-size: 10px; 
    font-weight: 600; 
    line-height: 20px;
}

.light-text {
    font-size: 10px; 
    font-weight: 400; 
    line-height: 20px;
}

.credit-section {
    display: flex;
    width: 100%;
    justify-content: center;
    padding: 10px 0px 20px 0px;
    font-size: 10px;
    font-weight: 600;
    line-height: 13px;
    background-color: #F9A438;
}

@media (max-width: 992px) {
    .my-container {
        padding: 60px 40px !important;
        gap: 20px;
    }

    .our-logo {
        height: 58px;
        width: auto;
        padding-bottom: 10px;
    }

    .identity-container {
        width: 100% !important;
        gap: 10px;
    }

    .light-text {
        width: 100%;
        text-align: center;
    }

    .hard-text {
        width: 100%;
        text-align: center;
    }
}
</style>