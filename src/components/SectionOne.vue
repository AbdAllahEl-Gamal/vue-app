<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <app-navigation></app-navigation>
        <div class="row play-for-purpose-row">
            <div class="col-6">
                <div class="play-for-purpose-section-par-cont">
                    <p class="play-for-purpose-text">Play<span class="four-number">4</span><br><span class="purpose-word">PURPOSE</span></p>
                    <div class="eclipse"></div>
                </div>
                <div class="join-now-btn">
                    <a>JOIN NOW <span class="join-now-right-arrows">>></span></a>
                </div>
                <div class="row games-images-section">
                    <div class="col-3">
                        <img src="Warzone.png">
                    </div>
                    <div class="col-3">
                        <img src="apexWhite.png">
                    </div>
                    <div class="col-3">
                        <img src="PUBG.png">
                    </div>
                </div>
            </div>
            <div class="col-6 soldier-section-col">
                <div class="soldier-section">
                    <img src="maskGroup.png">
                </div>
                <div class="small-spinner"></div>
                <div class="large-spinner"></div>
                <img src="Polygon1.png" class="polygon-image">
                <img src="Group4.png" class="x-image">
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
                        <p class="three-steps-text">{{ joinText }}</p>
                    </div>
                    <div class="col-4">
                        <p class="three-steps-number number-margin">02</p>
                        <p class="three-steps-title">PLAY</p>
                        <p class="three-steps-text">{{ playText }}</p>
                    </div>
                    <div class="col-4">
                        <p class="three-steps-number number-margin">03</p>
                        <p class="three-steps-title">EARN</p>
                        <p class="three-steps-text">{{ earnText }}</p>
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
            threeStepsBackgroundImage: { backgroundImage: "url(3easystepsbg.png)" },
            joinText: 'Subscribe to 365games.net and choose your membership (1, 3 or 6-months)',
            playText: 'Play your favorite battle royale game (COD Warzone, Apex Legend or Fortnite)',
            earnText: 'Earn up to 1 million dollars by playing tournaments or by lucky draws!'
        };
    },
    components: {
        AppNavigation
    },
    methods: {
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

.soldier-section-col {
    position: relative;
}

.soldier-section {
    position: relative;
    z-index: 1;
}

.soldier-section img {
    position: absolute;
    width: 100%;
    right: 22%;
    top: 30px;
    animation: glow 3s infinite alternate;
}

.join-now-btn {
    cursor: pointer;
    max-width: 325px;
    color: #ffffff !important;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-weight: 500;
    font-size: 23px;
    color: white;
    text-align: center;
    letter-spacing: 0.05em;
    clip-path: polygon(6% 0, 100% 0, 100% 20%, 100% 80%, 100% 100%, 0 100%, 0% 80%, 0 24%);
    margin-left: 8vw;
    margin-bottom: 5vw;
    border-style: solid;
    border-width: 4px;
    border-image: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%) 1;
    padding-top: 15px;
    padding-bottom: 15px;
    text-decoration: none !important;
}

.join-now-right-arrows {
    letter-spacing: -4px;
    padding-left: 20%;
}

.join-now-btn:hover {
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
}

.games-images-section {
    margin-left: 7.3vw;
}

.games-images-section img {
    max-width: 60%;
}

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
    background-clip: text;
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
    position: relative;
    z-index: 2;
    margin-bottom: 3vw;
}

.play-for-purpose-text {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 300;
    font-size: 10.5vw;
    line-height: 1.1em;
    letter-spacing: 0.01em;
    color: #FFFFFF;
    padding-left: 7.3vw;
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
    font-size: 10.5vw;
    letter-spacing: 0.01em;
    color: #FFFFFF;
}

.small-spinner {
    position: absolute;
    width: 480px;
    height: 480px;
    border: 4px solid #9672FF;
    border-top: 4px solid #6B4FE8;
    border-radius: 50%;
    border-style: solid;
    border-width: 7px;
    top: 13%;
    left: 3.7%;
    transition-duration: 5s;
    -webkit-transition-property: -webkit-transform;
    -webkit-transition-duration: 5s;
    -webkit-animation-name: rotate;
    -webkit-animation-iteration-count: infinite;
    -webkit-animation-timing-function: linear;
    -moz-transition-property: -moz-transform;
    -moz-animation-name: rotate; 
    -moz-animation-duration: 5s; 
    -moz-animation-iteration-count: infinite;
    -moz-animation-timing-function: linear;
    transition-property: transform;
    animation-name: rotate; 
    animation-duration: 5s; 
    animation-iteration-count: infinite;
    animation-timing-function: linear;
}

.large-spinner {
    position: absolute;
    width: 600px;
    height: 600px;
    border: 4px solid #9672FF;
    border-top: 4px solid #6B4FE8;
    border-radius: 50%;
    border-style: solid;
    border-width: 7px;
    right: 25%;
    top: 5%;
    transition-duration: 1.2;
    -webkit-transition-property: -webkit-transform;
    -webkit-transition-duration: 5s;
    -webkit-animation-name: rotate;
    -webkit-animation-iteration-count: infinite;
    -webkit-animation-timing-function: linear;
    -moz-transition-property: -moz-transform;
    -moz-animation-name: rotate; 
    -moz-animation-duration: 5s; 
    -moz-animation-iteration-count: infinite;
    -moz-animation-timing-function: linear;
    transition-property: transform;
    animation-name: rotate; 
    animation-duration: 5s; 
    animation-iteration-count: infinite;
    animation-timing-function: linear;
}

.polygon-image {
    position: absolute;
    right: 29%;
    top: 12%;
}

.x-image {
    position: absolute;
    right: 40%;
    top: 55%;
}

.polygon-image,
.x-image {
    transition-duration: 5;
    -webkit-transition-property: -webkit-transform;
    -webkit-transition-duration: 5s;
    -webkit-animation-name: rotate;
    -webkit-animation-iteration-count: infinite;
    -webkit-animation-timing-function: linear;
    -moz-transition-property: -moz-transform;
    -moz-animation-name: rotate; 
    -moz-animation-duration: 5s; 
    -moz-animation-iteration-count: infinite;
    -moz-animation-timing-function: linear;
    transition-property: transform;
    animation-name: rotate; 
    animation-duration: 5s; 
    animation-iteration-count: infinite;
    animation-timing-function: linear;
}

.eclipse {
    position: absolute;
    width: 30px;
    height: 30px;
    border: 4px solid transparent;
    border-top: 4px solid #6B4FE8;
    border-radius: 50%;
    border-style: solid;
    border-width: 3px;
    bottom: -27%;
    right: 20%;
    transition-duration: 1s;
    -webkit-transition-property: -webkit-transform;
    -webkit-transition-duration: 1s;
    -webkit-animation-name: rotate;
    -webkit-animation-iteration-count: infinite;
    -webkit-animation-timing-function: linear;
    -moz-transition-property: -moz-transform;
    -moz-animation-name: rotate; 
    -moz-animation-duration: 1s; 
    -moz-animation-iteration-count: infinite;
    -moz-animation-timing-function: linear;
    transition-property: transform;
    animation-name: rotate; 
    animation-duration: 1s; 
    animation-iteration-count: infinite;
    animation-timing-function: linear;
}

@-webkit-keyframes rotate {
    from { -webkit-transform: rotate(0deg); }
    to { -webkit-transform: rotate(360deg); }
}

@-moz-keyframes rotate {
    from { -moz-transform: rotate(0deg); }
    to { -moz-transform: rotate(360deg); }
}

@keyframes rotate {
    from { transform: rotate(0deg); }
    to { transform: rotate(360deg); }
}

@keyframes glow {
  from { opacity: 1; }
  to { opacity: 0.3; }
}
</style>