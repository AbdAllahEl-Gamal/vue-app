<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <app-navigation></app-navigation>
        <div class="row play-for-purpose-row">
            <div class="col-6">
                <div class="play-for-purpose-section-par-cont">
                    <p class="play-for-purpose-text">Play<span class="four-number">4</span><br><span class="purpose-word">PURPOSE</span></p>
                </div>
                <div class="join-now-btn-border-wrap">
                    <a class="join-now-btn">JOIN NOW <span class="join-now-right-arrows">>></span></a>
                </div>
                <div class="games-images-section">
                    <img src="Warzone.png">
                    <img src="apexWhite.png">
                    <img src="PUBG.png">
                </div>
            </div>
            <div class="col-6 soldier-section-col">
                <div class="soldier-section">
                    <img src="maskGroup.png">
                </div>
            </div>
        </div>
        <div class="row three-steps-row">
            <div :style="threeStepsBackgroundImage" class="three-steps-col">
                <p class="three-steps-header">3 Easy-Steps</p>
                <div class="row three-steps-content">
                        <!-- <img src="Rectangle6.png">
                        <img src="Group4.png">
                        <img src="Polygon1.png">
                        <img src="Rectangle7.png">
                        <img src="Vector2.png">
                        <img src="Vector2.png"> -->
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

.soldier-section-col {
    position: relative;
}

.soldier-section {
    position: absolute;
    right: 0;
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
    clip-path: polygon(6% 0, 100% 0, 100% 20%, 100% 80%, 100% 100%, 0 100%, 0% 80%, 0 24%);
    margin-left: 5vw;
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
    margin-left: 5vw;
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

.play-for-purpose-row {
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
    margin-bottom: 0px;
}

.three-steps-content {
    position: relative;
    top: 50%;
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
    max-width: 230px;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 300;
    font-size: 15px;
    text-align: left;
    line-height: 32px;
    color: #FFFFFF;
}

.play-for-purpose-section-par-cont {
    margin-bottom: 2vw;
}

.play-for-purpose-text {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 300;
    font-size: 10vw;
    line-height: 1.1em;
    letter-spacing: 0.01em;
    color: #FFFFFF;
    padding-left: 5vw;
}

.four-number {
    font-family: 'Poppins';
    font-style: italic;
    font-weight: bold;
    font-size: 11vw;
    letter-spacing: 0.01em;
    color: #9672FF;
}

.purpose-word {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 800;
    font-size: 10vw;
    letter-spacing: 0.01em;
    color: #FFFFFF;
}
</style>