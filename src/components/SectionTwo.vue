<template>
    <div :style="sectionBackgroundImage" class="container">
        
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
</style>