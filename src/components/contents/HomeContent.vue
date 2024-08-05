<template>
    <div class="my-container">
        <div class="my-background"></div>
        <div class="home">
            <div class="d-flex flex-column col-12 col-md-6" style="gap: 20px;">
                <div class="d-flex flex-column welcome-text">
                    <h2 class="welcome-text">
                        Transforming
                        your business.
                        <span style="color: #F37721;">Be our partner.</span>
                    </h2>
                </div>
                <div class="d-flex flex-column" style="gap: 20px;">
                    <b-button pill>APPLY FOR A JOB</b-button>
                    <b-button pill>REQUEST FOR <br> SERVICE CONSULTATION</b-button>
                </div>
            </div>
            <div></div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.home {
    position: relative;
    z-index: 2;
    display: flex;
    align-items: center;

    height: fit-content;
    padding: 80px 0px 100px 0px;
    margin: 0px 92px;
}

.welcome-text {
    font-size: 70px;
    font-weight: 600;
    line-height: 80px;

    color: white;
}

.my-container {
    position: relative;
    width: 100%;
    height: fit-content;
}

.my-background {
    background-image: url('@/assets/bg/mockup-videos.gif'); 
    background-size: contain; /* Adjust the background size */
    background-position: right center; /* Position the background in the right-center */
    background-repeat: no-repeat; /* Ensure the background doesn't repeat */
    width: 70%;
    height: 100%;
    position: absolute;
    top: 0;
    right: 0;
    z-index: 1; /* Background layer */
}

button {
    font-family: "Roboto", Sans-serif;
    font-size: 12px;
    font-weight: 600;

    width: 50%;

    padding: 12px 70px;

    border: none;
    background-color: white;
    color: black;
}

button:hover {
    background-color: #F37721;
    color: white;
}

@media (max-width: 992px) {
    .my-background {
        width: 100%;
        background-size: cover;
    }

    button {
        width: 100%;
    }
}
</style>