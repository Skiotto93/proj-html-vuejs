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
            currentIndex: 0,
            descriptions: [
                {
                    title: 'Our Team',
                    text: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil voluptates fuga hic reprehenderit eos? Doloremque, voluptate ipsum, fuga corporis vero nihil repellat eius voluptas deserunt a magni sapiente amet perferendis.',
                    image: '../img/rev-slider-main-home-img-03.jpg',
                },
                {
                    title: 'Our Job',
                    text: 'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Corporis, facere sit numquam molestiae nemo, esse voluptatum nisi nihil voluptate aut modi, iure iste dignissimos tempore? Veniam consectetur iure quibusdam enim?',                    
                    image: '../img/rev-slider-main-home-img-02.jpg',
                }
            ],
        }
    },
    methods: {
        nextIndex() {
            if ( this.currentIndex === this.descriptions.length - 1 ) {
                this.currentIndex = 0
            } else {
                this.currentIndex++
            }
        },
        prevIndex() {
            if ( this.currentIndex === 0 ) {
                this.currentIndex = this.descriptions.length - 1
            } else {
                this.currentIndex--
            }
        }
    }
}

</script>

<template>
    <header>
        <div class="carousel-images" v-for="(description, index) in descriptions">
            <img :src="description.image" :alt="description.title">
        </div> 
        <i class="fa-solid fa-arrow fa-arrow-right-long" @click="nextIndex"></i>
        <i class="fa-solid fa-arrow fa-arrow-left-long" @click="prevIndex"></i>
        <HeaderNavBar />
        <AppHeaderSon v-for="(description, index) in descriptions" 
        :title="description.title" :text="description.text" 
        :class="{inactive: index === currentIndex}"
        />
    </header>
</template>

<style lang="scss" scoped>
header {
    background-image: url('../img/rev-slider-main-home-img-03.jpg');
    background-position: center;
    background-size: cover;
    height: 890px;
    position: relative;
    .carousel-images {
        max-width: 100%;
    }
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
