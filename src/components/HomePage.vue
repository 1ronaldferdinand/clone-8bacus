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
        </div>
        <div id="events">
            <!-- Events content -->
        </div>
        <div id="careers">
            <!-- Careers content -->
        </div>
        <div id="news">
            <!-- News content -->
        </div>
        <div id="contact_us">
            <!-- Contact Us content -->
        </div>
    </div>
</template>
  
<script>
import NavBar from '@/components/NavBar.vue';
import SocialMedia from '@/components/SocialMedia.vue';
import HomeContent from '@/components/contents/HomeContent.vue';
import ServiceContent from '@/components/contents/ServiceContent.vue';
import AboutContent from '@/components/contents/AboutContent.vue';
  
export default {
    components: {
        NavBar,
        SocialMedia,
        HomeContent,
        ServiceContent,
        AboutContent,
    }
}
</script>