<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <div class="row newspaper-section">
            <div class="col-4 newspaper-soldier-section">
                <img src="newspaperSoldier.png" class="newspaper-soldier-image">
                <img src="Rectangle6.png" class="rectangle-image">
                <img src="Polygon1.png" class="polygon-image">
                <img src="Group4.png" class="x-image">
            </div>
            <div class="col-8 newspaper-soldier-form-section">
                <p class="header">Newsletter</p>
                <p class="header-text">{{ headerText }}</p>
                <div class="row email-input-btn-cont">
                    <input type="email" class="form-control newspaper-soldier-form-mail-input" id="inputEmail" placeholder="Enter your email">
                    <div class="subscribe-btn">
                        <a>Subscribe</a>
                    </div>
                </div>   
            </div>
        </div>
        <hr>
        <div class="row footer-section">
            <div class="col-4">
                <p class="copyright-par">©2022 <span class="purple-color">365games.</span> All Rights Reserved.</p>
            </div>
            <div class="col-4">
                <a class="footer-links">Advertise</a>
                <a class="footer-links">Sponsor</a>
                <a class="footer-links">Careers</a>
            </div>
            <div class="col-4">
                <a class="social-media-icons"><i class="fab fa-2x fa-facebook"></i></a>
                <a class="social-media-icons"><i class="fab fa-2x fa-twitter"></i></a>
                <a class="social-media-icons"><i class="fab fa-2x fa-instagram"></i></a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionFive',
    data() {
        return {
            sectionBackgroundImage: {backgroundImage: "url(newsletterBg.png)"},
            headerText: 'Get the latest updates about our new games and prizes'
        };
    },
    methods: {
    }
};
</script>

<style scoped>
.container-fluid {
    min-width: 100vh;
    background-color: #000000;
    background-repeat: no-repeat;
    background-size: 100% 100%;
    color: #ffffff;
    margin-bottom: -5px;
}

.newspaper-section {
    padding-bottom: 100px;
}

.newspaper-soldier-section {
    position: relative;
    margin-top: 20%;
}

.newspaper-soldier-section .newspaper-soldier-image {
    width: 100%;
    margin-top: 7%;
    animation: glow 3s infinite alternate;
}

.newspaper-soldier-section .rectangle-image {
    position: absolute;
    bottom: 0;
    left: 1%;
}

.newspaper-soldier-section .polygon-image {
    position: absolute;
    top: 10%;
    left: 24%;
}

.newspaper-soldier-section .x-image {
    position: absolute;
    top: 25%;
    right: 0;
}

.newspaper-soldier-form-section {
    margin-top: 43%;
}

.newspaper-soldier-form-section .header {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 800;
    font-size: 65px;
    line-height: 63px;
    letter-spacing: -0.5px;
    color: #ffffff;
    margin-left: 4%;
}

.newspaper-soldier-form-section .header-text {
    max-width: 100%;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    line-height: 50px;
    letter-spacing: -0.5px;
    opacity: 0.6;
}

.email-input-btn-cont {
    margin-left: 0px;
}

.newspaper-soldier-form-mail-input {
    display: inline-block;
    max-width: 280px !important;
    height: 55px !important;
    background-color: rgba(255, 255, 255, 0.08) !important;
    border: none !important;
    border-radius: 5px !important;
    color: #ffffff !important;
    margin-right: 20px;
}

.newspaper-soldier-form-mail-input::placeholder {
    color: #ffffff !important;
}

.newspaper-soldier-form-mail-input:focus {
    box-shadow: none !important;
}

.subscribe-btn {
    position: relative;
    cursor: pointer;
    max-width: 120px;
    color: #ffffff !important;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 18px;
    color: #ffffff;
    text-align: center;
    letter-spacing: -0.5px;
    clip-path: polygon(0 0, 84% 0, 100% 35%, 100% 80%, 100% 100%, 0 100%, 0% 80%, 0 24%);
    border-style: solid;
    border-width: 2px;
    border-image: linear-gradient(220deg, #9672FF 27.76%, rgba(107, 79, 232, 0) 94.18%) 1;
    border-radius: 5px;
    padding-top: 11px;
    padding-bottom: 11px;
    text-decoration: none !important;
    opacity: 0.8;
}

.subscribe-btn:hover {
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
}

.subscribe-btn:before {
    position: absolute;
    content: "";
    z-index: -1;
    top: -1px;
    right: 7px;
    bottom: 34px;
    -webkit-mask: linear-gradient(#ffffff 0 0) content-box, linear-gradient(#ffffff 0 0);
    mask: linear-gradient(#ffffff 0 0) content-box, linear-gradient(#ffffff 0 0);
    -webkit-mask-composite: xor;
    mask-composite: exclude;
    border-right: 3px solid #9672FF;
    transform: skew(+45deg);
}

hr {
    width: 76%;
    border: 0.5px solid #8080806b;
    margin: 0 auto;
    opacity: 0.1;
    margin-left: 10%;
}

.footer-section {
    text-align: center;
    padding-top: 20px;
    padding-bottom: 80px;
}

.copyright-par {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 0.6em;
    color: #ffffff;
    margin-bottom: 0px;
    margin-top: 0.8em;
}

.purple-color {
    color: #9672FF;
}

.footer-links {
    cursor: pointer;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 0.6em;
    text-decoration: none !important;
    color: #ffffff;
    margin-right: 30px;
}

.social-media-icons {
    cursor: pointer;
    margin-right: 20px;
    text-decoration: none;
}

.social-media-icons i {
    color: #ffffff;
    font-size: 16px;
}

.social-media-icons .fa-facebook:hover {
    color: #4267B2;
}

.social-media-icons .fa-twitter:hover {
    color: #00adb5;
}

.social-media-icons .fa-instagram:hover {
    color: #e11d74;
}

.newspaper-soldier-section .rectangle-image,
.newspaper-soldier-section .polygon-image,
.newspaper-soldier-section .x-image {
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
  from { opacity: 0.9; }
  to { opacity: 0.3; }
}
</style>