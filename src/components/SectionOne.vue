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
                <div class="large-spinner">
                    <div class="small-spinner"></div>
                </div>
                <img src="Polygon1.png" class="polygon-image">
                <img src="Group4.png" class="x-image">
            </div>
        </div>
        <div class="row three-steps-row">
            <div :style="threeStepsBackgroundImage" class="three-steps-col">
                <p class="three-steps-header">3 Easy-Steps</p>
                <div class="row h-100 justify-content-center align-items-center three-steps-content">
                    <div class="three-steps-shapes-cont">
                        <img src="Rectangle6.png" class="three-steps-shapes three-steps-rectangle1">
                    </div>
                    <div class="col-4 three-steps-content-col">
                        <p class="three-steps-number">01</p>
                        <p class="three-steps-title">JOIN</p>
                        <p class="three-steps-text">{{ joinText }}</p>
                        <img src="Vector2.png" class="three-steps-shapes three-steps-vector1">
                        <img src="Group4.png" class="three-steps-shapes three-steps-x-image">
                    </div>
                    <div class="col-4 three-steps-content-col">
                        <p class="three-steps-number number-margin">02</p>
                        <p class="three-steps-title">PLAY</p>
                        <p class="three-steps-text">{{ playText }}</p>
                        <img src="Vector2.png" class="three-steps-shapes three-steps-vector2">
                        <img src="Rectangle7.png" class="three-steps-shapes three-steps-rectangle2">
                        <img src="Polygon1.png" class="three-steps-shapes three-steps-polygon">
                    </div>
                    <div class="col-4 three-steps-content-col">
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
    height: 300vh;
    min-width: 100vh;
    background-color: black;
    background-repeat: no-repeat;
    color: #ffffff;
    margin-bottom: -5px;
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
}

.three-steps-content {
    position: relative;
    top: 20%;
}

.three-steps-content .three-steps-content-col {
    position: relative;
    text-align: center;
}

.three-steps-shapes-cont {
    position: absolute;
}

.three-steps-number {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 800;
    font-size: 6em;
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
    font-size: 3em;
    line-height: 32px;
    color: #FFFFFF;
}

.three-steps-text {
    max-width: 170px;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 300;
    font-size: 0.7em;
    text-align: left;
    line-height: 32px;
    color: #FFFFFF;
    margin: 0 auto;
    opacity: 0.7;
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
    width: 30vw;
    height: 30vw;
    border: 4px solid #9672FF;
    border-top: 4px solid #6B4FE8;
    border-radius: 50%;
    border-style: solid;
    border-width: 7px;
    top: 50%;
    left: 50%;
    margin: -15vw 0px 0px -15vw;
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
    width: 40vw;
    height: 40vw;
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

.three-steps-shapes {
    position: absolute;
}

.three-steps-vector1 {
    position: absolute;
    top: -45px;
    left: 64%;
}

.three-steps-vector2 {
    position: absolute;
    top: -45px;
    left: 64%;
}

.three-steps-rectangle1 {
    position: absolute;
    left: 6%;
    top: 15px;
}

.three-steps-rectangle2 {
    position: absolute;
    top: 40%;
    right: 75px;
}

.three-steps-polygon {
    position: absolute;
    top: -50px;
    right: -140px;
}

.three-steps-x-image {
    position: absolute;
    top: 30%;
    right: 40px;
}

.three-steps-shapes.three-steps-rectangle1,
.three-steps-shapes.three-steps-rectangle2,
.three-steps-shapes.three-steps-polygon,
.three-steps-shapes.three-steps-x-image {
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

@media only screen and (max-width: 768px) {
  /* For mobile phones: */
  .play-for-purpose-text {
    font-size: 7em;  
    padding-left: 20px;
  }
  .four-number {
    font-size: 1em;
  }
  .purpose-word {
    font-size: 0.7em;
  }
  .join-now-btn {
    max-width: 180px;
    padding-top: 7px;
    padding-bottom: 7px;
  }
  .join-now-right-arrows {
    padding-left: 3%;
  }
  .large-spinner {
    width: 300px;
    height: 300px;
  }
  .small-spinner {
    width: 250px;
    height: 250px;
    margin: -125px 0px 0px -125px;
  }
  .polygon-image {
    top: 3%;
  }
  .x-image {
    top: 30%;
  }
  .eclipse {
    bottom: -33%;
  }
  .three-steps-text {
    max-width: 100px;
    font-size: 0.4em;
    line-height: 15px;
  }
  .three-steps-vector1, .three-steps-vector2 {
    width: 50%;
    top: 90px;
    left: 73%;
  }
  .three-steps-x-image {
    width: 7%; 
    top: 45%;
    right: 20px;
  }
  .three-steps-rectangle1 {
    width: 5%;
    top: 45px;
    left: 15px;
  }
  .three-steps-rectangle2 {
    width: 7%;
    top: 44%;
    right: 20px;
  }
  .three-steps-polygon {
    width: 7%;
    top: 85px;
    right: -45px;
  }
}
</style>