<script>

export default {
    name: 'AppJumbo',

    data() {
        return {

        }
    },
    methods: {


    },


    mounted() {

    }

}
</script>

<template>
    <div class="bg">

        <div id="video" class="container-fluid bg-warning my_container g-0 p-0 ">
            <!-- VIDEO SECTION  -->
            <div class="my_videoSection p-0 m-0 g-0 debug">
                <video muted="" autoplay="" loop="" src="/src/assets/Login_Food Reel FH Studio.mp4" type="video/mp4"
                    class="my_Video debug">
                    <img class="debug" src="/src/assets/errorVideo.png" alt="Error Video">
                </video>
            </div>
        </div>
    </div>
</template>

<style scoped>
.debug{
    border: 2px dashed blue;
}
.my_container {
    height: 100vh;
}

.my_videoSection {
    height: 100vh;

}
.bg{
    background-color: rgba(33, 37, 41, 0.5) !important;
border: 2px dashed blue;
}

.my_Video {
    height: 100vh;
    width: 100%;
    object-fit: cover;
    display: block;
}

@media screen and (max-width: 992px) {}
</style>