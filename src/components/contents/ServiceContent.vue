<template>
    <div>
        <div class="my-container">
            <div class="top-background"></div>
            <div class="service-text-area">
                <h2 class="service-text">What we <span style="color:#F37721"> offer? </span></h2>
            </div>
        </div>
        <div class="my-card-container">
            <div class="my-card">
                <div class="d-flex flex-column align-items-center" style="gap: 20px;">
                    <div>
                        <img height="100" src="@/assets/icons/8b-icon-0001.png" alt="">													
                    </div>
                    <div class="my-card-title-container">
                        <span class="my-card-title">RECRUITMENT</span>		
                    </div>
                    <div>
                        <p>Our team of recruitment offers recruitment services to help organizations find and hire the right talent.</p>						
                    </div>
                </div>
                <div>
                    <b-button pill>Request for Proposal</b-button>
                </div>
            </div>

            <div class="my-card">
                <div class="d-flex flex-column align-items-center" style="gap: 20px;">
                    <div>
                        <img height="100" src="@/assets/icons/8b-icon-0002.png" alt="">													
                    </div>
                    <div class="my-card-title-container">
                        <span class="my-card-title">ADMINISTRATIVE</span>		
                    </div>
                    <div>
                        <p>Our team of administrative offers administrative support services that can significantly enhance the efficiency and productivity of the business of our clients.</p>						
                    </div>
                </div>
                <div>
                    <b-button pill>Request for Proposal</b-button>
                </div>
            </div>

            <div class="my-card">
                <div class="d-flex flex-column align-items-center" style="gap: 20px;">
                    <div>
                        <img height="100" src="@/assets/icons/8b-icon-0004.png" alt="">													
                    </div>
                    <div class="my-card-title-container">
                        <span class="my-card-title">IMMIGRATION</span>		
                    </div>
                    <div>
                        <p>We offers comprehensive visa and work permit application services designed to streamline and simplify the process for an organization.</p>						
                    </div>
                </div>
                <div>
                    <b-button pill>Request for Proposal</b-button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.service-text-area {
    position: relative;
    z-index: 2;
    display: flex;
    align-items: center;
    justify-content: center;

    height: 280px;
}

.service-text {
    color: #000000;
    font-family: "Roboto", Sans-serif;
    font-size: 48px;
    font-weight: 600;
}

.my-container {
    position: relative;
    width: 100%;
    height: fit-content;
}

.top-background {
    background-image: url('@/assets/bg/background2-scaled.jpg'); 
    background-size: cover; /* Adjust the background size */
    background-position: center; /* Position the background in the center */
    background-repeat: no-repeat; /* Ensure the background doesn't repeat */
    width: 100%;
    height: 300px;
    position: absolute;
    top: 0;
    left: 0;
    z-index: 1;
}

.my-card-container {
    padding: 50px 0px; 
    margin: 0px 75px;
    display: flex;
    justify-content: center;

    gap: 20px;
}

.my-card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    padding: 10px;

    height: 350px;
    width: 273px;

    transition: transform 0.3s, opacity 0.3s, border 0.3s, border-radius 0.3s;
}

.my-card:hover {
    transform: scale(1.15);
    opacity: 0.5;
    border: 2px solid #F37721;
    border-radius: 8px;
}

.my-card p {
    text-align: center;
    font-size: 12px;
    font-family: "Roboto", Sans-serif;
}

.my-card-title {
    color: #000000;
    font-family: "Roboto", Sans-serif;
    font-size: 16px;
    font-weight: 600;
}

.my-card-title-container {
    border-bottom: 1px solid black;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px 0px;
}

button {
    font-family: "Roboto", Sans-serif;
    font-size: 12px;
    font-weight: 600;

    width: 100%;
    padding: 8px 24px;
    border: none;
    background-color: #F4D926;
    color: black;
}

button:hover {
    background-color: #F37721;
    color: white;
}
</style>