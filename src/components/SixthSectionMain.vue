<script>
import { def } from '@vue/shared';


export default {
    name: 'SixthSectionMain',
    data() {
        return {
            currentImage: 0,
            testimonials: [
                {
                    name: 'Cynthia Clark',
                    image: '../img/h3-img-04.png',
                    text: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Neque suscipit, expedita nemo'
                },
                {
                    name: 'Amanda Ming',
                    image: '../img/h3-img-07.png',
                    text: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate officiis optio eius.'
                },
                {
                    name: 'Priscilla Oswald',
                    image: '../img/h3-img-08.png',
                    text: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium voluptas, cumque ducimus.'
                }
            ]
        }
    },
    methods: {
        nextIndex() {
            if ( this.currentImage === this.testimonials.length - 1 ) {
                this.currentImage = 0
            } else {
                this.currentImage++
            }
        },
        prevIndex() {
            if ( this.currentImage === 0 ) {
                this.currentImage = this.testimonials.length - 1
            } else {
                this.currentImage--
            }
        },
    },
}
</script>

<template>
    <section>
        <div class="containerBackground">
            <p>Testimonials.</p>
        </div>
        <div class="cards">
            <i class="fa-solid fa-arrow-right-long" @click="nextIndex"></i>
            <i class="fa-solid fa-arrow-left-long" @click="prevIndex"></i>
            <div class="card" 
            v-for="(testimonial, index) in testimonials"
            :class="{active: index === currentImage}"
            v-show=" index == currentImage "
            >
                <img :src="testimonial.image" :alt="testimonial.name">
                <h3>{{ testimonial.name }}</h3>
                <p>"{{ testimonial.text }}"</p>
                <div class="progress-container">
                    <span class="first">{{ index + 1 }}</span>
                    <progress max="100"></progress>    
                    <span class="second">{{ testimonials.length }}</span>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #1e1c1c;
    position: relative;
    .containerBackground {
        color: black;
        position: absolute;
        top: 18%; 
        right: 55%;
        transform: translate(50%,-50%);
        margin: auto;
        max-width: 1400px;
        p {
            font-size: 300px;
        }
    }
    .cards {
        padding: 120px 0;
        text-align: center;
        max-width: 500px;
        margin: auto;
        .fa-arrow-left-long, .fa-arrow-right-long {
            position: absolute;
            top: 50%;
            font-size: 30px;
        }
        .fa-arrow-left-long:hover, .fa-arrow-right-long:hover {
            color: #fff;
        }
        .fa-arrow-left-long {
            left: 90px;
        }
        .fa-arrow-right-long {
            right: 90px;
        }
        .active {
            display: block;
        }
        .card {
            width: 300px;
            margin: auto;
            padding: 20px;
            h3 {
                padding: 30px 0;
                color: #fff;
            }
            p {
                color: #737272;
            }
            progress {
                position: relative;
                height: 5px;
                margin-top: 40px;
            }
            progress::before,
            progress::after {
                content: "";
                position: absolute;
                top: 0;
                left: 0;
                height: 100%;
            }
            progress::before {
                width: 100%;
                background: #4b4949;
            }
            progress::after {
                width: 33%;
                background: #fff;
            }
            .first, .second {
                color: #fff;
                margin: 0 30px;
            }
        }
    }
    .progress-container {
        border-radius: 10px;
        display: flex;
        align-items: flex-end;
    
    }
}
</style>