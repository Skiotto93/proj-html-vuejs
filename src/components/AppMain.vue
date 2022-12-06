<script>
import FirstSectionMain from './FirstSectionMain.vue';
import SecondSectionMain from './SecondSectionMain.vue';
import ThirdSectionMain from './ThirdSectionMain.vue';
import FourthSectionMain from './FourthSectionMain.vue';
import FifthSectionMain from './FifthSectionMain.vue';



export default {
    name: 'AppMain',
    components: {
        FirstSectionMain,
        SecondSectionMain,
        ThirdSectionMain,
        FourthSectionMain,
        FifthSectionMain,

    },
}
</script>

<template>
    <FirstSectionMain />
    <SecondSectionMain />
    <ThirdSectionMain />
    <FourthSectionMain />
    <FifthSectionMain />

</template>

<style lang="scss" scoped>

</style>