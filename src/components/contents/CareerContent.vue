<template>
    <div>
        <div class="my-container" style="padding-top: 100px;">
            <h2 class="service-text">Careers</h2>
            <div class="careers-container">
                <div class="row">
                    <div
                        class="column"
                        v-for="(career, index) in careers"
                        :key="index"
                    >
                        <button class="career-button">{{ career }}</button>
                    </div>
                </div>
            </div>
        </div>
        <div class="mid-background"></div>
        <div class="my-container flex-row justify-content-center" style="padding: 50px 160px; gap: 50px;">
            <img src="@/assets/images/8b-image-0001.jpg" width="50%">
            <div class="d-flex flex-column why-area w-50">
                <span>Why Should You Choose Us?</span>
                <p>
                    Welcome to 8Bacus Corp., where excellence meets innovation. 
                    We pride ourselves on being the driving force behind your business success by providing unmatched recruitment, admin, and visa services. 
                    Choose us for a seamless journey toward growth and efficiency.
                </p>
                <b-button pill>Request for Proposal</b-button>
            </div>
        </div>
        <div class="bot-background"></div>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            careers: [
                'Front-End Developers',
                'Back-End Developers',
                'UI/UX Designer',
                'Sale Support Specialist',
                'E-Commerce Marketer',
                'Key Accounts Manager'
            ]
        };
    }
};
</script>
  
<style scoped>
.careers-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}
  
.row {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
}
  
.column {
    padding: 5px;
    width: 30%;
}
  
.career-button {
    background-color: #ff9900; /* Adjust color as needed */
    color: black;
    border: none;
    border-radius: 10px; /* Adjust border radius as needed */
    padding: 10px 20px;
    font-family: "Roboto", Sans-serif;
    font-size: 16px;
    font-weight: 500;
    display: flex;
    align-items: center;
    justify-content: space-between;
    cursor: pointer;
    width: 100%;
}
  
.career-button::after {
    content: '➔'; /* Unicode for right arrow */
    margin-left: 10px;
}
  
.career-button:hover {
    background-color: #e68a00; /* Adjust hover color as needed */
}
  
.my-container {
    padding: 50px 80px;
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
  
.mid-background {
    background-image: url('@/assets/bg/background5.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    width: 100%;
    height: 300px;
    border: none;
}

.bot-background {
    background-image: url('@/assets/bg/background8.png');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    width: 100%;
    height: 300px;
    border: none;
}

button {
    font-family: "Roboto", Sans-serif;
    font-size: 12px;
    font-weight: 600;

    width: fit-content;
    padding: 8px 32px;
    border: none;
    background-color: #F4D926;
    color: black;
}

button:hover {
    background-color: #F37721;
    color: white;
}

.why-area {
    gap: 20px;
}

.why-area span {
    color: #F2D926;
    font-family: "Roboto", sans-serif;
    font-size: 28px;
    font-weight: 600;
    line-height: 28px;
}

.why-area p {
    color: black;
    font-family: "Roboto", sans-serif;
    font-size: 13px;
    font-weight: 400;
    line-height: 20px;
}
</style>  