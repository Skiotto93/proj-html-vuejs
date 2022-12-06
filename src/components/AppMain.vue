<script>
import FirstSectionMain from './FirstSectionMain.vue';
import SecondSectionMain from './SecondSectionMain.vue';
import ThirdSectionMain from './ThirdSectionMain.vue';
import FourthSectionMain from './FourthSectionMain.vue';
import FifthSectionMain from './FifthSectionMain.vue';
import SixthSectionMain from './SixthSectionMain.vue';
import SeventhSectionMain from './SeventhSectionMain.vue';
import LastSectionMainVue from './LastSectionMain.vue';

export default {
    name: 'AppMain',
    components: {
        FirstSectionMain,
        SecondSectionMain,
        ThirdSectionMain,
        FourthSectionMain,
        FifthSectionMain,
        SixthSectionMain,
        SeventhSectionMain,
        LastSectionMainVue
    },
}
</script>

<template>
    <FirstSectionMain />
    <SecondSectionMain />
    <ThirdSectionMain />
    <FourthSectionMain />
    <FifthSectionMain />
    <SixthSectionMain />
    <SeventhSectionMain />
    <LastSectionMainVue />
</template>

<style lang="scss" scoped>

</style>