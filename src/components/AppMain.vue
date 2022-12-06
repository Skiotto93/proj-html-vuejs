<script>
import FirstSectionMain from './FirstSectionMain.vue';
import SecondSectionMain from './SecondSectionMain.vue';
import ThirdSectionMain from './ThirdSectionMain.vue';
import FourthSectionMain from './FourthSectionMain.vue';
import FifthSectionMain from './FifthSectionMain.vue';
import SixthSectionMain from './SixthSectionMain.vue';
import SeventhSectionMain from './SeventhSectionMain.vue';

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
</template>

<style lang="scss" scoped>

</style>