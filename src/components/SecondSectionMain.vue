<script>
export default {
    name: 'SecondSectionMain',
}
</script>

<template>
    <section>
        <div class="container">
            <img src="../img/h1-img-01.jpg" alt="#">
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
        padding-top: 300px;
        display: flex;
        position: relative;
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
                font-size: 25px;
                background-color: #ff4c19;
                color: white;
                width: 40px;
                height: 40px;
                border-radius: 50%;
                line-height: 40px;
                text-align: center;
                margin-right: 10px;
            }
        }
    }
}
</style>