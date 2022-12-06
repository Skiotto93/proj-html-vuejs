<script>
export default {
    name: 'SeventhSectionMain'
}
</script>

<template>
    <section>
        <img src="../img/h1-img-04.jpg" alt="#">
        <i class="fa-solid fa-play"></i>
        <div class="circle">
            <img src="../img/svg-8.svg" alt="#">
        </div>
        <div class="cart">
            <img src="../img/svg-7.svg" alt="#">
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    position: relative;
    .fa-play {
        margin: 0;
        position: absolute;
        top: 50%;
        left: 50%;
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
        color: #fff;
        font-size: 40px;
    }
    .fa-play:hover {
        color: #ff4612;
    }
    .cart {
        width: 45px;
        height: 45px;
        position: absolute;
        top: 50px;
        right: 0;
        background-color: #fff;
        line-height: 50px;
        text-align: center;
        img {
            width: 15px;
            height: 15px;
        }
    }
    .cart:hover {
        background-color: #ef2853;
        img {
            filter: brightness(0) invert(1);
        }
    }
    .circle {
        width: 45px;
        height: 45px;
        position: absolute;
        top: 0;
        right: 0;
        background-color: #ef2853;
        line-height: 55px;
        text-align: center;
        img {
            width: 25px;
            height: 25px;
            filter: brightness(0) invert(1);
        }
    }
    .circle:hover {
        background-color: #fff;
        img {
            filter: none;
        }
    }
}
</style>