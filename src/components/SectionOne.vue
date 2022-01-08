<template>
    <div class="container">
        <app-navigation></app-navigation>
        <div class="row">
            <div class="col-6 left-image-section">
                <img src="playForPurpose.png"> 
            </div>
            <div class="col-6 right-image-section">
                <img src="365Screen11.png"> 
            </div>
        </div>
        <div class="row">
            <div class="col-12 icons-section">
                <img src="pngkitFortnitePngLogo4308881.png"> 
                <img src="warzoneLogoWhiteTmAtvi2.png"> 
                <img src="apexWhite2.png"> 
                <img src="pngItem11648122.png"> 
            </div>
        </div>
    </div>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';
export default {
    name: 'SectionOne',
    components: {
        AppNavigation
    }
};
</script>

<style scoped>
.container {
    height: 115vh;
    max-width: 100vw;
    min-width: 100vw;
    background-color: black;
    color: #ffffff;
    padding: 0px;
    margin: 0px;
    overflow-x: hidden;
}

.left-image-section {
    padding-top: 145px;
}

.left-image-section img {
    width: 62%;
    margin-left: 16%;
}

.right-image-section {
    position: relative;
}

.right-image-section img {
    position: absolute;
    top: -49%;
    right: -4%;
    width: 130%;
}

.icons-section {
    text-align: center;
    margin-top: 13%;
}

.icons-section img {
    margin-right: 12%;
}
</style>