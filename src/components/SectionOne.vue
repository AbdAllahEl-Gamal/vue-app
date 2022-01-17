<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <app-navigation></app-navigation>
        <div class="row">
            <div class="col-12 section-one-col">
                <div class="play-for-purpose-section">
                    <img src="Play4PURPOSE.png" class="play-for-purpose-image">
                    <div class="join-now-btn-border-wrap">
                        <a class="join-now-btn">JOIN NOW <span class="join-now-right-arrows">>></span></a>
                    </div>
                    <!-- <div class="test-div">
                        JOIN NOW <span class="join-now-right-arrows">>></span>
                    </div> -->
                    <div class="games-images-section">
                        <img src="Warzone.png">
                        <img src="apexWhite.png">
                        <img src="PUBG.png">
                    </div>
                </div>
                <div class="soldier-section">
                    <img src="maskGroup.png">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';
export default {
    name: 'SectionOne',
    data() {
        return {
            sectionBackgroundImage: {backgroundImage: "url(headerBg.png)"}
        };
    },
    components: {
        AppNavigation
    }
};
</script>

<style scoped>
.container-fluid {
    height: 1445px;
    min-width: 100vh;
    background-color: black;
    background-repeat: no-repeat;
    color: #ffffff;
}

.section-one-col {
    position: relative;
}

.play-for-purpose-section {
    position: absolute;
    top: 2px;
    left: 79px;
    z-index: 3;
}

.play-for-purpose-section .play-for-purpose-image {
    width: 100%;
}

.soldier-section {
    position: absolute;
    top: -20px;
    left: 600px;
    z-index: 2;
}

.soldier-section img {
    width: 100%;
}

.join-now-btn-border-wrap {
    max-width: 231px;
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
    padding: 1px !important;
    color: #ffffff !important;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-weight: 500;
    font-size: 23px;
    letter-spacing: 0.05em;
    margin-top: 80px;
    clip-path: polygon(6% 0, 100% 0, 100% 20%, 100% 80%, 100% 100%, 0 100%, 0% 80%, 0 24%);
}

.join-now-btn {
    cursor: pointer;
    background: #000000;
    color: white;
    padding-right: 25px !important;
    padding-left: 25px !important;
    text-decoration: none !important;
}

.join-now-right-arrows {
    padding-left: 30px;
    letter-spacing: -4px;
}

.join-now-btn:hover {
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
}

.games-images-section {
    margin-top: 80px;
}

.games-images-section img {
    margin-right: 80px;
}

/* .test-div {
    position: relative;
    width: 30%;
    margin: 0 auto;
    overflow: hidden;
    padding: 10px;
    text-align: center;
    color: #ffffff !important;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-weight: 500;
    font-size: 23px;
    letter-spacing: 0.05em;
    clip-path: polygon(6% 0, 100% 0, 100% 20%, 100% 80%, 100% 100%, 0 100%, 0% 80%, 0 24%);
    background: white;
} */
</style>