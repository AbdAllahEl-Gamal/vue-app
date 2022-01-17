<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <app-navigation></app-navigation>
        <div class="row play-for-purpose-col">
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
        <div class="row three-steps-row">
            <div :style="threeStepsBackgroundImage" class="three-steps-col">
                <p class="three-steps-header">3 Easy-Steps</p>
                <div class="row three-steps-content">
                    <div class="col-4">
                        <p class="three-steps-number">01</p>
                        <p class="three-steps-title">JOIN</p>
                        <p class="three-steps-text">Subscribe to 365games.net and choose your membership (1, 3 or 6-months)</p>
                    </div>
                    <div class="col-4">
                        <p class="three-steps-number number-margin">02</p>
                        <p class="three-steps-title">PLAY</p>
                        <p class="three-steps-text">Play your favorite battle royale game (COD Warzone, Apex Legend or Fortnite)</p>
                    </div>
                    <div class="col-4">
                        <p class="three-steps-number number-margin">03</p>
                        <p class="three-steps-title">EARN</p>
                        <p class="three-steps-text">Earn up to 1 million dollars by playing tournaments or by lucky draws!</p>
                    </div>
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
            sectionBackgroundImage: { backgroundImage: "url(headerBg.png)" },
            threeStepsBackgroundImage: { backgroundImage: "url(3easystepsbg.png)" }
        };
    },
    components: {
        AppNavigation
    }
};
</script>

<style scoped>
.container-fluid {
    height: 290vh;
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

.play-for-purpose-col {
    height: 100vh;
}

.three-steps-row {
    height: 100vh;
}

.three-steps-col {
    background-size: 100% 100%;
    background-repeat: no-repeat;
}

.three-steps-header {
    position: relative;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 800;
    font-size: 80px;
    text-align: center;
    color: #FFFFFF;
    -webkit-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
    top: 50%;
    margin-bottom: 5%;
}

.three-steps-content {
    position: relative;
    text-align: center;
    -webkit-transform: translateY(-50%);
    -ms-transform: translateY(-50%);
    transform: translateY(-50%);
    top: 57%;
}

.three-steps-number {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 800;
    font-size: 140px;
    line-height: 110px;
    background: linear-gradient(180deg, #9471FC 0%, #886FCF 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-shadow: 0 0 0 black;
    -webkit-text-stroke: 0.1px #9471FC;
}

.three-steps-title {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 900;
    font-size: 47px;
    line-height: 32px;
    color: #FFFFFF;
}

.three-steps-text {
    width: 230px;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 300;
    font-size: 15px;
    text-align: left;
    line-height: 32px;
    color: #FFFFFF;
    margin-left: 39%;
}

.number-margin {
    margin-left: 30px;
}
</style>