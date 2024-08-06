<template>
    <div>
        <div class="my-container">
            <h2 class="service-text">News</h2>
            <div class="news-container">
                <div class="news-card" v-for="(news, index) in newsItems" :key="index">
                    <div class="image-container">
                        <div style="padding: 20px 0px;">
                            <img :src="news.image" alt="news image" class="news-image"/>
                        </div>
                        <div class="overlay">
                            <b-icon-arrow-right style="color: white;"></b-icon-arrow-right>
                        </div>
                    </div>
                    <div class="news-content h-100">
                        <h3 class="news-title">{{ news.title }}</h3>
                        <p class="news-description">{{ news.description }}</p>
                        <a href="#" class="news-read-more">Read More</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    data() {
        return {
            newsItems: [
                {
                    image: require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                    title: 'Tech Talent Has Growing Expectations: Will Employers Rise to the Challenge?',
                    description: 'What happens when tech talent teams, used to analyzing data...',
                },
                {
                    image: require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                    title: '10 Communication Strategies to Better Engage Candidates',
                    description: 'Engaging candidates effectively is crucial in today’s competitive recruitment landscape...',
                },
                {
                    image: require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                    title: 'The Impact of Bad Hires and How to Prevent Them',
                    description: 'While finding the right person to join an organization is...',
                },
                {
                    image: require('@/assets/images/developing-programmer-team-development-website-design-coding-technologies.jpg'),
                    title: 'Empowering Candidates to Shape Their Recruitment Journey',
                    description: 'In the quest to create a more engaging recruitment process...',
                },
            ],
        };
    },
  };
</script>
  
<style scoped>
.news-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}
  
.news-card {
    background-color: white;
    border: 1px solid #ddd;
    overflow: hidden;
    width: 23%; 
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    display: flex;
    flex-direction: column;
}
  
.image-container {
    position: relative;
}
  
.news-image {
    width: 100%;
    height: auto;
    display: block;
}
  
.overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.6);
    display: flex;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: opacity 0.3s;
}
  
.arrow-icon {
    width: 50px;
    height: 50px;
}
  
.image-container:hover .overlay {
    opacity: 1;
}

.news-content {
    padding: 15px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100%;
}

.news-title {
    font-family: "Roboto", Sans-serif;
    font-size: 14px;
    font-weight: 600;
    line-height: 16px;
    color: black;
    margin-bottom: 10px;
}
  
.news-description {
    font-family: "Roboto", Sans-serif;
    font-size: 12px;
    line-height: 14px;
    color: #555;
    margin-bottom: 10px;
    flex-grow: 1;
}
  
.news-read-more {
    font-family: "Roboto", Sans-serif;
    font-size: 14px;
    color: #007bff;
    text-decoration: none;
    align-self: flex-start;
}

.news-read-more:hover {
    text-decoration: underline;
}
  
.my-container {
    padding: 100px 80px;
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
</style>