<template>
    <div style="height: 100%;">
        <SocialMedia />
        <NavBar />
        
        <div id="home" class="bg-black">
            <HomeContent/>
        </div>
        <div id="services">
            <ServiceContent/>
        </div>
        <div id="about_us">
            <AboutContent/>
            <IndustryContent/>
        </div>
        <div id="events">
            <EventContent/>
        </div>
        <div id="careers">
            <CareerContent/>
        </div>
        <div id="news">
            <NewsContent/>
        </div>
        <ContactContent/>
        <FooterPage/>
    </div>
</template>
  
<script>
import NavBar from '@/components/NavBar.vue';
import SocialMedia from '@/components/SocialMedia.vue';
import HomeContent from '@/components/contents/HomeContent.vue';
import ServiceContent from '@/components/contents/ServiceContent.vue';
import AboutContent from '@/components/contents/AboutContent.vue';
import IndustryContent from '@/components/contents/IndustryContent.vue';
import EventContent from '@/components/contents/EventContent.vue';
import CareerContent from '@/components/contents/CareerContent.vue';
import NewsContent from '@/components/contents/NewsContent.vue';
import ContactContent from '@/components/contents/ContactContent.vue';
import FooterPage from '@/components/FooterPage.vue';

export default {
    components: {
        NavBar,
        SocialMedia,
        HomeContent,
        ServiceContent,
        AboutContent,
        IndustryContent,
        EventContent,
        CareerContent,
        NewsContent,
        ContactContent,
        FooterPage,
    }
}
</script>