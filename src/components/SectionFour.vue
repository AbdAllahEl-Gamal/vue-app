<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <div class="row newspaper-section">
            <div class="col-4 newspaper-soldier-section">
                <img src="newspaperSoldier.png">
            </div>
            <div class="col-8 newspaper-soldier-form-section">
                <img src="Heading.png">
                <p>Get the latest updates about our new games and prizes</p>
                <input type="email" class="form-control newspaper-soldier-form-mail-input" id="inputEmail" placeholder="Enter your email">  
                <button class="subscribe-btn">S</button>    
            </div>
        </div>
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
                <a class="social-media-icons"><img src="Facebook.png"></a>
                <a class="social-media-icons"><img src="Twitter.png"></a>
                <a class="social-media-icons"><img src="Instagram.png"></a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionFive',
    data() {
        return {
            sectionBackgroundImage: {backgroundImage: "url(newsletterBg.png)"}
        };
    },
};
</script>

<style scoped>
.container-fluid {
    min-width: 100vh;
    background-color: black;
    background-repeat: no-repeat;
    color: #ffffff;
}

.newspaper-section {
    padding-bottom: 100px;
}

.newspaper-soldier-section {
    margin-top: 20%;
}

.newspaper-soldier-section img {
    width: 100%;
    margin-left: 17px;
}

.newspaper-soldier-form-section {
    margin-top: 43%;
}

.newspaper-soldier-form-section img {
    padding-left: 5%;
}

.newspaper-soldier-form-section p {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 17px;
    line-height: 50px;
    letter-spacing: -0.5px;
    opacity: 0.6;
}

.newspaper-soldier-form-mail-input {
    display: inline-block;
    width: 330.58px !important;
    height: 65.55px !important;
    background-color: rgba(255, 255, 255, 0.08) !important;
    border: none !important;
    border-radius: 5px !important;
    color: #ffffff !important;
}

.newspaper-soldier-form-mail-input::placeholder {
    color: #ffffff !important;
}

.newspaper-soldier-form-mail-input:focus {
    box-shadow: none !important;
}

.subscribe-btn {
    
}

.footer-section {
    text-align: center;
    padding-bottom: 100px;
}

.copyright-par {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    color: #FFFFFF;
}

.purple-color {
    color: #9672FF;
}

.footer-links {
    cursor: pointer;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 16px;
    text-decoration: none !important;
    color: #FFFFFF;
    margin-right: 30px;
}

.social-media-icons {
    cursor: pointer;
    text-decoration: none !important;
    margin-right: 20px;
}
</style>