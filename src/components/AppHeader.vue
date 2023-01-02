<script>
import AppHeaderSon from './AppHeaderSon.vue';
import HeaderLinks from './HeaderLinks.vue';
import HeaderNavBar from './HeaderNavBar.vue';

export default {
    name: 'AppHeader',
    components: {
        AppHeaderSon,
        HeaderLinks,
        HeaderNavBar,
    },
    data() {
        return {
            description: {
                title: 'Our Team',
                text: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil voluptates fuga hic reprehenderit eos? Doloremque, voluptate ipsum, fuga corporis vero nihil repellat eius voluptas deserunt a magni sapiente amet perferendis.'
            }
        }
    }
}

</script>

<template>
    <header>
        <i class="fa-solid fa-arrow fa-arrow-right-long"></i>
        <i class="fa-solid fa-arrow fa-arrow-left-long"></i>
        <HeaderNavBar />
        <AppHeaderSon :title="description.title" :text="description.text"/>
    </header>
</template>

<style lang="scss" scoped>
header {
    background-image: url('../img/rev-slider-main-home-img-03.jpg');
    background-position: center;
    background-size: cover;
    height: 890px;
    position: relative;
    .fa-arrow {
            font-size: 30px;
            position: absolute;
            bottom: calc(50% - 30px);
            cursor: pointer;
        }
        .fa-arrow:hover {
            color: #ff4c19;
        }
        .fa-arrow-right-long {
            right: 100px;
        }
        .fa-arrow-left-long {
            left: 100px;
        }
    
}

</style>
