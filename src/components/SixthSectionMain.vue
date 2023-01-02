<script>
import { def } from '@vue/shared';

export default {
    name: 'SixthSectionMain',
}
</script>

<template>
    <section>
        <i class="fa-solid fa-arrow-right-long"></i>
        <i class="fa-solid fa-arrow-left-long"></i>
        <div class="containerBackground">
            <p>Testimonials.</p>
        </div>
        <div class="cards">
            <div class="card">
                <img src="../img/h3-img-04.png" alt="#">
                <h3>Cynthia Clark</h3>
                <p>"Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate officiis optio eius."</p>
                <div class="progress-container">
                    <span class="first">01</span>
                    <progress value="33" max="100"></progress>    
                    <span class="second">03</span>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #1e1c1c;
    position: relative;
    z-index: -2;
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
    .containerBackground {
            color: black;
            position: absolute;
            top: 18%; 
            right: 55%;
            transform: translate(50%,-50%);
            margin: auto;
            max-width: 1400px;
            z-index: -1;
            p {
                font-size: 300px;
            }
    }
    .cards {
        padding: 120px 0;
        text-align: center;
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
            .progress-container {
                border-radius: 10px;
                display: flex;
                align-items: flex-end;
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
    }
}
</style>