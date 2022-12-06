<script>
export default {
    name: 'FourthSectionMain',
}
</script>

<template>
    <section>
        <div class="container">
            <div class="col-left">
                <h1>Creative Leader<span class="orangePoint">.</span></h1>
                <div class="line"></div>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem omnis officia minima eius voluptates facilis neque odio iste suscipit asperiores doloremque, nisi similique enim assumenda error nihil reprehenderit ut voluptas!</p>
                <h4>READ MORE</h4>
            </div>
            <div class="col-right">
                <div class="d-flex">
                    <h3>Mentorship</h3>
                    <span class="bar">78%</span>
                </div>
                <div class="line78"></div>
                <div class="d-flex">
                    <h3>Education</h3>
                    <span class="bar">95%</span>
                </div>
                <div class="line95"></div>
                <div class="d-flex">
                    <h3>Learning</h3>
                    <span class="bar">65%</span>
                </div>
                <div class="line65"></div>
                <div class="d-flex">
                    <h3>Motivation</h3>
                    <span class="bar">83%</span>
                </div>
                <div class="line83"></div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
section {
    margin: auto;
    max-width: 1450px;
    padding: 100px;
    .container {
        display: flex;
        .col-left {
            width: 50%;
            padding: 40px;
            .line {
                width: 70px;
                border-bottom: 1px solid #ff4612;
                padding-top: 20px;
            }
            p {
                padding: 20px 0;
            }
            h4 {
                padding-top: 10px;
            }
        }
        .col-right {
            width: 50%;
            padding: 40px;
            .d-flex {
                display: flex;
                justify-content: space-between;
                .bar {
                    font-weight: bold;
                }
            }
            h3 {
                padding-bottom: 10px;
            }
            .line78 {
                width: 78%;
                border-bottom: 3px solid #ff4612;
                margin-bottom: 30px;
            }
            .line95 {
                width: 95%;
                border-bottom: 3px solid #ff4612;
                margin-bottom: 30px;
            }
            .line65 {
                width: 65%;
                border-bottom: 3px solid #ff4612;
                margin-bottom: 30px;
            }
            .line83 {
                width: 83%;
                border-bottom: 3px solid #ff4612;
                margin-bottom: 30px;
            }
        }
    }
}
</style>