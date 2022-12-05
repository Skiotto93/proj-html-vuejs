<script>
import FirstSectionMain from './FirstSectionMain.vue';
import SecondSectionMain from './SecondSectionMain.vue';
import ThirdSectionMain from './ThirdSectionMain.vue'

export default {
    name: 'AppMain',
    components: {
        FirstSectionMain,
        SecondSectionMain,
        ThirdSectionMain
    },
}
</script>

<template>
    <FirstSectionMain />
    <SecondSectionMain />
    <ThirdSectionMain />
</template>

<style lang="scss" scoped>

</style>