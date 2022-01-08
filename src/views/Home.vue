<template>
    <div>
        <SectionOne></SectionOne>
        <SectionTwo></SectionTwo>
        <SectionThree></SectionThree>
        <SectionFour></SectionFour>
        <SectionFive></SectionFive>
    </div>
</template>

<script>
import SectionOne from '@/components/SectionOne';
import SectionTwo from '@/components/SectionTwo';
import SectionThree from '@/components/SectionThree';
import SectionFour from '@/components/SectionFour';
import SectionFive from '@/components/SectionFive';

export default {
    name: 'home',
    components: {
        SectionOne,
        SectionTwo,
        SectionThree,
        SectionFour,
        SectionFive
    }
};
</script>