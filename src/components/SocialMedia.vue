<template>
    <div class="social-media">
        <div class="social-media-item">
            <b-icon-facebook variant="secondary" style="width: 24px; height: 24px;"></b-icon-facebook>
        </div>
        <div class="social-media-item">
            <b-icon-instagram variant="secondary" style="width: 24px; height: 24px;"></b-icon-instagram>
        </div>
        <div class="social-media-item">
            <b-icon-linkedin variant="secondary" style="width: 24px; height: 24px;"></b-icon-linkedin>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.social-media {
    position: fixed;
    top: 50%;
    left: 0;
    transform: translateY(-50%);
    display: flex;
    flex-direction: column;
    justify-content: center;
    z-index: 9999;
}

.social-media-item{
    cursor: pointer;
    padding: 12px;
}

.social-media-item:hover {
    background-color: black;
    padding-left: 30px;
}
</style>