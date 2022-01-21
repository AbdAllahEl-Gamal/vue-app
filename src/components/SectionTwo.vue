<template>
    <div :style="sectionBackgroundImage" class="container-fluid">
        <div class="row section-three-row">
            <div class="col-6">
                <div class="left-section">
                    <div class="symbol-cont">
                        <img src="symbol.png" class="symbol-image">
                        <p class="left-section-header">What<br>Players Say</p>
                    </div>
                    <div class="left-section-comment-cont">
                        <div class="left-section-icon-cont">
                            <img src="Icon1.png" class="left-section-comment-icon">
                        </div>
                        <span class="left-section-quote-mark-span">
                            <img src="quoteMark.png">
                        </span>
                        <p class="left-section-comment-par">{{ leftComment }}</p>
                        <p class="left-section-comment-author">{{ leftCommentAuthor }}</p>
                        <p class="left-section-comment-role">{{ leftCommentRole }}</p>
                    </div>
                </div>                
            </div>
            <div class="col-6">
                <div class="right-section">
                    <div class="right-section-comment1-cont">
                        <div class="right-section-comment1-icon-cont">
                            <img src="ogLogo.png" class="right-section-comment1-icon">
                        </div>
                        <span class="right-section-comment1-quote-mark-span">
                            <img src="quoteMark.png">
                        </span>
                        <p class="right-section-comment1-par">{{ rightComment1 }}</p>
                        <p class="right-section-comment1-author">{{ rightComment1Author }}</p>
                        <p class="right-section-comment1-role">{{ rightComment1Role }}</p>
                    </div>
                    <div class="right-section-comment2-cont">
                        <div class="right-section-comment2-icon-cont">
                            <img src="LGD.png" class="right-section-comment2-icon">
                        </div>
                        <span class="right-section-comment2-quote-mark-span">
                            <img src="quoteMark.png">
                        </span>
                        <p class="right-section-comment2-par">{{ rightComment2 }}</p>
                        <p class="right-section-comment2-author">{{ rightComment2Author }}</p>
                        <p class="right-section-comment2-role">{{ rightComment2Role }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionThree',
    data() {
        return {
            sectionBackgroundImage: { backgroundImage: "url(testimonials.png)" },
            leftComment: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation.',
            leftCommentAuthor: 'Jesper Wecksell',
            leftCommentRole: 'Player, Fanatic Team',
            rightComment1: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.',
            rightComment1Author: 'Matthea Wünsch',
            rightComment1Role: 'Manager, Team Liquid',
            rightComment2: '365 games gave us a new generation of gaming',
            rightComment2Author: 'Wang Chunyu',
            rightComment2Role: 'Leader, LGD Gaming'
        };
    },
    methods: {
    }
};
</script>

<style scoped>
.container-fluid {
    height: 160vh;
    min-width: 100vh;
    background-color: #000000;
    background-repeat: no-repeat;
    background-size: 100% 100%;
    color: #ffffff;
    margin-bottom: -5px;
}

.left-section {
    position: relative;
    float: right;
}

.symbol-cont {
    margin-bottom: 65px;
}

.symbol-image {
    position: absolute;
    left: -145px;
    top: -85px;
}

.left-section-header {
    position: relative;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: 800;
    font-size: 65px;
    line-height: 64px;
    color: #ffffff;
    text-align: left;
}

.left-section-comment-cont {
    max-width: 416px;
    min-height: 436px;
    background: #ffffff;
    border-radius: 15px;
    padding: 40px;
}

.left-section-comment-par {
    max-width: 304px;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    line-height: 32px;
    color: #18191F;
    text-align: left;
    padding-left: 50px;
    padding-top: 5px;
    margin-bottom: 25px;
}

.left-section-comment-icon {
    text-align: left;
}

.left-section-comment-author {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0px !important;
    padding-left: 20px;
}

.left-section-comment-role {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    color: #969BAB;
    padding-left: 20px;
}

.left-section-quote-mark-span {
    float: left;
}

.left-section-icon-cont {
    margin-bottom: 15px;
    margin-left: 22px;
}

.right-section-comment1-cont {
    max-width: 509px;
    min-height: 360px;
    background: #ffffff;
    border-radius: 15px;
    padding: 40px;
    margin-top: 35px;
}

.right-section-comment1-icon-cont {
    margin-bottom: 15px;
    margin-left: 22px;
}

.right-section-comment1-icon {
    text-align: left;
}

.right-section-comment1-quote-mark-span {
    float: left;
}

.right-section-comment1-par {
    max-width: 445px;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    line-height: 32px;
    color: #18191F;
    text-align: left;
    padding-left: 50px;
    padding-top: 5px;
    margin-bottom: 25px;
}

.right-section-comment1-author {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0px !important;
    padding-left: 20px;
}

.right-section-comment1-role {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    color: #969BAB;
    padding-left: 20px;
}

.right-section-comment2-cont {
    max-width: 350px;
    min-height: 300px;
    background: #ffffff;
    border-radius: 15px;
    padding: 40px;
    margin-top: 35px;
}

.right-section-comment2-icon-cont {
    margin-bottom: 15px;
    margin-left: 22px;
}

.right-section-comment2-icon {
    text-align: left;
}

.right-section-comment2-quote-mark-span {
    float: left;
}

.right-section-comment2-par {
    max-width: 230px;
    font-family: 'Poppins';
    font-style: normal;
    font-weight: normal;
    font-size: 18px;
    line-height: 32px;
    color: #18191F;
    text-align: left;
    padding-left: 50px;
    padding-top: 5px;
    margin-bottom: 25px;
}

.right-section-comment2-author {
    font-family: 'Poppins';
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    background: linear-gradient(180deg, #9672FF 0%, #6B4FE8 100%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 0px !important;
    padding-left: 20px;
}

.right-section-comment2-role {
    font-family: 'Inter';
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    color: #969BAB;
    padding-left: 20px;
}
</style>