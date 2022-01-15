<template>
    <div :style="sectionBackgroundImage" class="container">
        <div class="row">
            <div class="col-12 steps-title-section">
                <img src="section3StepsTitle.png">
            </div>
        </div>
        <div class="row steps-section">
            <div class="col-4">
            </div>
            <div class="col-4">
            </div>
            <div class="col-4">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionTwo',
    data() {
        return {
            sectionBackgroundImage: {backgroundImage: "url(3easystepsbg.png)"}
        };
    },
};
</script>

<style scoped>
.container {
    height: 950px;
    width: 1672px;
    background-color: black;
    background-repeat: no-repeat;
    color: #ffffff;
}

.steps-title-section {
    text-align: center;
}

.steps-section {
    text-align: center;
}
</style>