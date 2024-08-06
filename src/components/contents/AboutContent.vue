<template>
    <div>
        <div class="top-background"></div>
        <div class="my-card-container">
            <div class="col-6 d-flex justify-content-center">
                <img height="360" src="@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg" alt="">
            </div>
            <div class="col-6 d-flex flex-column justify-content-between">
                <div class="d-flex justify-content-center">
                    <div class="about-us-text position-relative">
                        <span class="about-text">About</span>
                        <span class="us-text">Us</span>
                    </div>
                </div>
                <p class="about-us-description">
                    We understand that success in today’s dynamic business environment requires the right talent, seamless administrative support, and expert visa services. As your dedicated partner, we bring unparalleled expertise to streamline your operations and empower your growth journey.
                </p>
            </div>
        </div>
        <div class="d-flex align-items-center" style="gap: 8px; justify-content: space-around; padding: 0px 8px; padding-bottom: 32px;">
            <div class="line-spacer w-100"></div>
            <span class="what-sets-up w-100 text-center">
                What Sets Us Apart?
            </span>
            <div class="line-spacer w-100"></div>
        </div>
        <div class="d-flex flex-column flex-md-row align-items-center align-items-md-start justify-content-start justify-content-md-center" style="padding: 10px 0px;">
            <div class="my-card">
                <img height="172" src="@/assets/icons/8b-icon-0005.png" alt="">													
                <span class="my-card-title">Industry Expertise</span>
                <p class="text-center" style="font-size: 12px; margin: 0px 20px;">
                    Benefit from our in-depth knowledge of diverse industries. 
                    We tailor our services to meet the specific demands of your sector, 
                    ensuring a customized and effective approach.
                </p>
            </div>

            <div class="my-card">
                <img height="172" src="@/assets/icons/8b-icon-0006.png" alt="">													
                <span class="my-card-title">Client-Centric Approach</span>
                <p class="text-center" style="font-size: 12px; margin: 0px 20px;">
                    Your goals are our goals. 
                    We take the time to understand your objectives, 
                    tailoring our services to align with your vision. 
                    Your success story is at the heart of everything we do.
                </p>
            </div>

            <div class="my-card">
                <img height="172" src="@/assets/icons/8b-icon-0007.png" alt="">													
                <span class="my-card-title">Technology-Driven Approach</span>
                <p class="text-center" style="font-size: 12px; margin: 0px 20px;">
                    Embrace innovation with our technology-driven solutions. 
                    We leverage cutting-edge tools to enhance efficiency and provide you with a competitive edge.
                </p>
            </div>
        </div>
        <div class="d-flex flex-column flex-md-row align-items-center align-items-md-start justify-content-start justify-content-md-center" style="padding: 10px 0px;">
            <div class="my-card">
                <img height="172" src="@/assets/icons/8b-icon-0008.png" alt="">													
                <span class="my-card-title">Transparent Processes</span>
                <p class="text-center" style="font-size: 12px; margin: 0px 20px;">
                    Trust is paramount. 
                    We maintain transparency in our processes, 
                    keeping you informed every step of the way. 
                    Your peace of mind is our priority.
                </p>
            </div>

            <div class="my-card">
                <img height="172" src="@/assets/icons/8b-icon-0009.png" alt="">													
                <span class="my-card-title">Tailored Solutions</span>
                <p class="text-center" style="font-size: 12px; margin: 0px 20px;">
                    One size does not fit all. 
                    Our solutions are customized to meet the unique needs of your business. 
                    Your success story is our top priority.
                </p>
            </div>
        </div>
        <div class="other-services d-flex flex-column-reverse flex-lg-row">
            <div class="col-12 col-md-10 section-container">
                <div class="section step-1">
                    <span style="font-size: 18px; font-weight: 600; line-height: 18px;">
                        Strategic Recruitment
                    </span>
                    <p style="font-size: 12px; font-weight: 400; line-height: 20px;">
                        Elevate your workforce with our strategic recruitment solutions. 
                        We go beyond just filling positions 
                        – we find the perfect match for your company culture and objectives, 
                        ensuring long-term success.
                    </p>
                </div>
                <div class="section step-2">
                    <span style="font-size: 18px; font-weight: 600; line-height: 18px;">
                        Effortless Administration
                    </span>
                    <p style="font-size: 12px; font-weight: 400; line-height: 20px;">
                        Say goodbye to administrative hassles. 
                        Our comprehensive admin services cover everything from documentation management to HR support, 
                        allowing you to focus on your core business functions.
                    </p>
                </div>
                <div class="section step-3">
                    <span style="font-size: 18px; font-weight: 600; line-height: 18px;">
                        Visa Expertise
                    </span>
                    <p style="font-size: 12px; font-weight: 400; line-height: 20px;">
                        Navigating visa processes can be a labyrinth. 
                        Let our visa experts guide you through the complexities, 
                        offering reliable and timely services for individuals and businesses alike.
                    </p>
                </div>
            </div>
            <div class="col-12 d-block d-lg-none" style="text-align: center; line-height: 24px;">
                Unlock Your
                Business
                Potential with
                <span style="color:#F37721; font-weight:600;">
                    8Bacus Corp.
                </span>
                Your
                Complete
                Solutions
                Partner!
            </div>
            <div class="col-2 d-none d-lg-block" style="text-align: end; line-height: 42px;">
                Unlock Your<br>
                Business<br>
                Potential with<br>
                <span style="color:#F37721; font-weight:600;">
                    8Bacus Corp.<br>
                </span>
                Your<br>
                Complete<br>
                Solutions<br>
                Partner!<br>
            </div>
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.service-text {
    color: black;
    font-family: "Roboto", Sans-serif;
    font-size: 48px;
    font-weight: 600;
}

.my-container {
    position: relative;
    width: 100%;
    height: fit-content;
}

.my-card-container {
    padding: 50px 0px 150px 0px; 
    margin: 0px 75px;
    display: flex;
    justify-content: center;

    gap: 20px;
}

.about-us-text {
    color: #000000;
    font-family: "Roboto", Sans-serif;
    font-size: 155px;
    font-weight: 600;
    letter-spacing: -4px;

    position: relative;
    display: inline-block;
}

.about-text {
    display: inline-block;
    position: relative;
}

.us-text {
    position: absolute;
    top: 78%; /* Adjust as needed */
    left: 62%; /* Adjust as needed */
    color: #f37b33;
    transform: translate(-50%, -50%);
}

.about-us-description {
    text-align: center; 
    font-family: 'Roboto', Sans-serif; 
    font-size: 13px;
}

.top-background {
    background-image: url('@/assets/bg/background5.png'); 
    background-size: cover; /* Adjust the background size */
    background-position: center; /* Position the background in the center */
    background-repeat: no-repeat; /* Ensure the background doesn't repeat */
    width: 100%;
    height: 300px;
}

.line-spacer {
    border-bottom: 1px solid #F37721;
}

.what-sets-up {
    color: black; 
    font-family: 'Roboto', Sans-serif; 
    font-size: 28px; 
    font-weight: 600;
}

.my-card-title {
    color: #F37721;
    font-family: "Roboto", Sans-serif;
    font-size: 16px;
    font-weight: 600;
}

.my-card {
    height: 380;
    width: 370px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: 10px;
    gap: 20px;
}

.other-services {
    color: #000000;
    font-family: "Roboto", Sans-serif;
    font-size: 20px;
    font-weight: 400;
    line-height: 46px;
    padding: 100px 120px;
}

.section-container {
  display: flex;
  flex-direction: column;
  align-items: start;
}

.section {
    max-width: 480px;
    text-align: start;
    position: relative;
}

.section.step-1 {
    left: 0;
}

.section.step-2 {
    left: 90px; /* Adjust as needed */
}

.section.step-3 {
    left: 180px; /* Adjust as needed */
}

@media (max-width: 992px){
    .other-services {
        padding: 100px 80px;
        gap: 20px
    }

    .section.step-2 {
        left: 0; /* Adjust as needed */
    }

    .section.step-3 {
        left: 0; /* Adjust as needed */
    }
}
</style>