<template>
    <div :style="sectionBackgroundImage" class="container">
        <div class="row">
            <div class="col-4 newspaper-soldier-section">
                <img src="newspaperSoldier.png">
            </div>
            <div class="col-8 newspaper-soldier-form-section">
                <img src="Heading.png">
                <p>
                    Get the latest updates about our new games and prizes 
                </p>      
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
.container {
    height: 1000px;
    width: 1672px;
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
</style>