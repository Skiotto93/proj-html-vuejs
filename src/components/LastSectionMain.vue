<script>
export default {
    name: 'LastSectionMain'
}
</script>

<template>
    <section>
        <div class="col-left">
            <img class="worldMap" src="../img/h1-contact-rev-01.png" alt="#">
            <img class="findNewYork" src="../img/h1-contact-rev-02.png" alt="#">
            <img class="findMelburne" src="../img/h1-contact-rev-02.png" alt="#">
            <img class="findLondon" src="../img/h1-contact-rev-02.png" alt="#">
            <div class="description">
                <h3>New York Coaching</h3>
                <h4>READ MORE</h4>
            </div>
        </div>
        <div class="col-right">
            <div class="info">
                <h1>Contact us<span class="orangePoint">.</span></h1>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Iste tenetur</p>
                <div class="line"></div>
            </div>
            <form class="text-input">
                <div class="user">
                    <input class="name" type="text" placeholder="Your Name">
                    <input class="email" type="email" placeholder="Your Email">
                    <input class="text" type="text" placeholder="Write a message...">
                </div>
                <button type="button" class="button-orange">
                    SEND
                    <div>
                        <i class="fa-solid fa-arrow-right-long"></i>
                    </div>
                </button>
            </form>
        </div>
    </section>
    <div class="clients">
        <img src="../img/h4-clients-img-04-1.png" alt="#">
        <img src="../img/h4-clients-img-06-1.png" alt="#">
        <img src="../img/h4-clients-img-08-1.png" alt="#">
        <img src="../img/h4-clients-img-10-1.png" alt="#">
        <img src="../img/h4-clients-img-02.png" alt="#">
    </div>
</template>

<style lang="scss" scoped>
section {
    max-width: 1380px;
    margin: auto;
    padding: 120px 0 60px 0;
    display: flex;
    .col-left {
        width: 40%;
        position: relative;
        padding: 20px;
        .worldMap {
            width: 100%;
        }
        .findNewYork {
            position: absolute;
            top: 37%;
            left: 25%;
        }
        .findMelburne {
            position: absolute;
            right: 18%;
            bottom: 25%;
        }
        .findLondon {
            position: absolute;
            top: 30%;
            left: 43%;
        }
        .description {
            background-color: #fff;
            padding: 15px;
            box-shadow: 2px 5px 10px #888888;
            position: absolute;
            top: 48%;
            left: 23%;
            opacity: 0.8;
        }
    }
    .col-right {
        width: 60%;
        h1 {
            font-size: 30px;
        }
        p {
            padding: 15px 0;
        }
        .line {
            width: 70px;
            border-bottom: 2px solid #ff4c19;
        }
        .user {
            padding: 20px 0;
            .name, .email {
                padding: 10px 10px;
                border: none;
                border-bottom: 1px solid;
                width: calc(50% - 10px);
            }
            .name {
                margin-right: 10px;
            }
            .text {
                margin-top: 10px;
                padding-bottom: 40px;
                padding-top: 10px;
                padding-left: 10px;
                width: calc(100% - 10px);
                border: none;
                border-bottom: 1px solid;
            }
            
        }
        .button-orange {
                padding: 10px;
                margin-top: 20px;
                background-color: #ff4c19;
                color: #fff;
                display: flex;
                border: none;
                cursor: pointer;
                div {
                    margin-left: 20px;
                    padding-left: 10px;
                    border-left: 1px solid;
                }
                div:hover {
                    border-left: inherit;
                }
            }
    }
}
.clients {
    margin: auto;
    max-width: 1400px;
    display: flex;
    justify-content: space-between;
    padding-bottom: 60px;
    img {
        filter: brightness(0);
    }
    img:hover {
        filter: none;
    }
}
</style>