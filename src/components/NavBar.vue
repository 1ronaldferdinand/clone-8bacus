<template>
    <div>
        <b-navbar toggleable="md" type="dark" variant="dark" class="bg-black my-navbar sticky-top">
            <b-navbar-brand to="#home">
                <img src="@/assets/cropped-top-logo-head.png" alt="Logo" height="40" class="d-inline-block align-top">
            </b-navbar-brand>
    
            <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    
            <b-collapse id="nav-collapse" is-nav>
                <b-navbar-nav class="ml-auto">
                    <b-nav-item to="#home" exact>Home</b-nav-item>
                    <b-nav-item to="#services">Services</b-nav-item>
                    <b-nav-item to="#about_us">About Us</b-nav-item>
                    <b-nav-item to="#events">Events</b-nav-item>
                    <b-nav-item to="#careers">Careers</b-nav-item>
                    <b-nav-item to="#news">News</b-nav-item>
                    <b-nav-item to="#contact_us">Contact Us</b-nav-item>
                </b-navbar-nav>
            </b-collapse>
        </b-navbar>
    </div>
</template>
  
<script>  
export default {

}
</script>

<style>
.nav-link {
    color: white;
}
</style>

<style scoped>
.my-navbar {
    width: 100%;
    padding: 20px !important;
}
  
.b-navbar-nav .nav-item .nav-link {
    color: white !important;
    font-size: 1.2rem; 
}
  
.b-navbar-nav .nav-item .nav-link:hover {
    color: lightblue !important;
}

.navbar-expand-md .navbar-collapse {
    justify-content: flex-end;
}
  
.brand-text {
    color: white;
    font-size: 1.5rem; 
    margin-left: 10px;
}

.sticky-top {
    position: fixed;
    top: 0;
    z-index: 99999;
}
</style>
  