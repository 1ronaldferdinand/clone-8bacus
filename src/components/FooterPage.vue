<template>
    <div class="d-flex flex-column align-items-center">
        <div class="d-flex align-items-start justify-content-between w-100" style="padding: 64px 100px;">
            <div class="d-flex flex-column align-items-center col-4" style="gap: 10px;">
                <div class="d-flex flex-column" style="width: fit-content;">
                    <img src="@/assets/cropped-top-logo-head.png" height="40" width="150">
                    <span class="light-text">
                        We go beyond services; we provide<br> solutions that empower your business to<br> thrive.
                    </span>
                    <div class="d-flex flex-column">
                        <span class="hard-text">Company landline number:</span>
                        <span class="light-text">02-53104708</span>
                    </div>
                </div>
            </div>
            <div class="col-3 d-flex flex-column">
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
            <div class="col-3 d-flex flex-column">
                <span class="hard-text" style="font-size: 16px; padding-bottom: 10px;">Legal</span>
                <div class="light-text">
                    Privacy Policy<br>
                    Terms and Conditions<br>
                </div>
            </div>
            <div class="col-2 d-flex flex-column align-items-center gap-2">
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
</style>