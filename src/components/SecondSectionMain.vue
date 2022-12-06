<script>
export default {
    name: 'SecondSectionMain',
}
</script>

<template>
    <section>
        <div class="container">
            <img class="bkg-circle" src="../img/svg-4.svg" alt="#">
            <img src="../img/h1-img-01.jpg" alt="#">
            <button class="buttonOtange">
                <i class="fa-solid fa-arrow-left-long"></i>
                <i class="fa-solid fa-arrow-right-long"></i>
            </button>
            <div class="container-small">
                <h1>Jason Bickford</h1>
                <span>Founder and Executive Director</span>
                <div class="line">_________</div>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsum rem dolor sint ut consequuntur, alias asperiores quidem minima id ratione...</p>
                <div class="icons">
                    <i class="fa-brands fa-linkedin-in"></i>
                    <i class="fa-brands fa-facebook-f"></i>
                    <i class="fa-brands fa-twitter"></i>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    background-color: #fafafa;
    padding-bottom: 140px;
    .container {
        max-width: 1300px;
        margin: auto;
        padding-top: 600px;
        display: flex;
        position: relative;
        .bkg-circle {
            position: absolute;
            right: -200px;
            top: 45%;
        }
        .buttonOtange {
            position: absolute;
            bottom: 0;
            left: 0;
            padding: 15px 30px;
            background-color: #ff4c19;
            border: none;
            cursor: pointer;
            i {
                font-size: 30px;
                color: #fafafa;
            }
            i:first-child {
                margin-right: 10px;
            }
        }
        .container-small {
            background-color: #fff;
            display: flex;
            flex-direction: column;
            justify-content: center;
            height: 400px;
            width: 700px;
            padding: 0 50px;
            position: absolute;
            right: -100px;
            bottom: 90px;
            h1 {
                font-size: 40px;
            }
            span, p {
                color: #919191;
            }
            .line, .icons {
                color: #ff4c19;
                padding: 25px 0;
            }
            .icons i {
                font-size: 15px;
                background-color: #ff4c19;
                color: white;
                width: 30px;
                height: 30px;
                border-radius: 50%;
                line-height: 30px;
                text-align: center;
                margin-right: 10px;
            }
            .icons i:hover {
                background-color: #1e1e1e;
            }
        }
    }
}
</style>