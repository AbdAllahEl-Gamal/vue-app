<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <div class="row">
            <div class="col-4 newspaper-soldier-section">
                <img src="newspaperSoldier.png">
            </div>
            <div class="col-8 newspaper-soldier-form-section">
                <img src="Heading.png">
                <p>Get the latest updates about our new games and prizes</p>
                <input type="email" class="form-control newspaper-soldier-form-mail-input" id="inputEmail" placeholder="Enter your email">      
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
    width: 330.58px !important;
    height: 65.55px !important;
    background-color: rgba(255, 255, 255, 0.08) !important;
    border: none !important;
    border-radius: 5px !important;
    color: #ffffff !important;
}

.newspaper-soldier-form-mail-input:focus {
    box-shadow: none !important;
}
</style>