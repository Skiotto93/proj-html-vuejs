<script>
export default {
    name: 'FifthSectionMain'
}
</script>

<template>
    <section>
        <img class="bkg-circle" src="../img/svg-4.svg" alt="#">
        <div class="text">
            <h1>Latest news<span class="orangePoint">.</span></h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
            <div class="line"></div>
        </div>
        <div class="cards">
            <i class="fa-solid fa-arrow-left-long"></i>
            <i class="fa-solid fa-arrow-right-long"></i>
            <div class="card">
                <div class="image">
                    <img id="firstImage" src="../img/h1-blog-img-02.jpg" alt="#">
                    <img id="secondImage" src="../img/h1-blog-img-03.jpg" alt="#">
                    <div class="ticket">
                        <i class="fa-solid fa-tag"></i>
                        <span>Business, Leading</span>
                    </div>
                </div>
                <div class="date">
                    <i class="fa-regular fa-clock"></i>
                    <span>May 5, 2019</span>
                    <i class="fa-regular fa-user"></i>
                    <span>Amanda Doe</span>
                </div>
                <h2>Next Investment</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum inventore beatae numquam. Magnam, aliquid esse...</p>
                <h4>READ MORE</h4>
            </div>
            <div class="card">
                <div class="image">
                    <img id="firstImage" src="../img/h1-blog-img-03.jpg" alt="#">
                    <img id="secondImage" src="../img/h1-blog-img-04.jpg" alt="#">
                    <div class="ticket">
                        <i class="fa-solid fa-tag"></i>
                        <span>Business, Leading</span>
                    </div>
                </div>
                <div class="date">
                    <i class="fa-regular fa-clock"></i>
                    <span>May 5, 2019</span>
                    <i class="fa-regular fa-user"></i>
                    <span>Amanda Doe</span>
                </div>
                <h2>Team Building</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum inventore beatae numquam. Magnam, aliquid esse...</p>
                <h4>READ MORE</h4>
            </div>
            <div class="card">
                <div class="image">
                    <img id="firstImage" src="../img/h1-blog-img-04.jpg" alt="#">
                    <img id="secondImage" src="../img/h1-blog-img-01.jpg" alt="#">
                    <div class="ticket">
                        <i class="fa-solid fa-tag"></i>
                        <span>Business, Leading</span>
                    </div>
                </div>
                <div class="date">
                    <i class="fa-regular fa-clock"></i>
                    <span>May 5, 2019</span>
                    <i class="fa-regular fa-user"></i>
                    <span>Amanda Doe</span>
                </div>
                <h2>New Business</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ipsum inventore beatae numquam. Magnam, aliquid esse...</p>
                <h4>READ MORE</h4>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #fafafa;
    position: relative;
    .bkg-circle {
        position: absolute;
        top: -80px;
        left: 5%;
    }
    .text {
        text-align: center;
        padding: 70px 0;
        h1 {
            font-size: 40px;
        }
        .line {
            width: 70px;
            border-bottom: 1px solid #ff4612;
            margin: auto;
        }
        p {
            padding: 30px 0;
            font-size: 18px;
            color: #9b9b9b;
        }
    }
    .cards {
        width: 1400px;
        margin: auto;
        padding: 30px;
        display: flex;
        .fa-arrow-left-long, .fa-arrow-right-long {
        position: absolute;
        bottom: 35%;
        font-size: 30px;
        }
        .fa-arrow-right-long {
            right: 100px;
        }
        .fa-arrow-right-long:hover, .fa-arrow-left-long:hover {
            color: #ff4612;
        }
        .fa-arrow-left-long {
            left: 100px;
        }
        .card {
            width: calc(100% / 3 - 20px);
            padding: 20px;
            .image {
                position: relative;
                margin-bottom: 30px;
                .ticket {
                    padding: 10px;
                    background-color: #ff4612;
                    color: #ffab93;
                    position: absolute;
                    right: 20px;
                    bottom: -15px;
                    i {
                        padding-right: 10px;
                    }
                }
                .ticket:hover {
                    color: #fafafa;
                }
            }
            #firstImage {
                width: 100%;
            }
            #secondImage {
                width: 100%;
                height: 170px;
                object-fit: cover;
                object-position: bottom;
                position: absolute;
                bottom: 0;
                left: 0;
            }
            .date i {
                color: #ff4612;
                padding-right: 10px;
            }
            .date span {
                padding-right: 10px;
                padding-top: 20px;
                color: #9b9b9b;
            }
        h2 {
                padding: 20px 0;
            }
    }
        p {
            color: #9b9b9b;
            padding-bottom: 30px;
        }
    }
}
</style>