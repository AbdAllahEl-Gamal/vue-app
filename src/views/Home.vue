<template>
    <div>
        <SectionOne></SectionOne>
        <SectionTwo></SectionTwo>
        <SectionThree></SectionThree>
        <SectionFour></SectionFour>
    </div>
</template>

<script>
import SectionOne from '@/components/SectionOne';
import SectionTwo from '@/components/SectionTwo';
import SectionThree from '@/components/SectionThree';
import SectionFour from '@/components/SectionFour';

export default {
    name: 'home',
    components: {
        SectionOne,
        SectionTwo,
        SectionThree,
        SectionFour
    }
};
</script>