<script>
export default {
    name: 'FirstSectionMain',
    data() {
        return {
            cards: [
                {
                    image: '../img/clessidra.png',
                    title: 'Knowing',
                },
                {
                    image: '../img/logo-side-area-img-01-1.png',
                    title: 'Selling',
                },
                {
                    image: '../img/pen-and-paper.png',
                    title: 'Learning',
                },
                {
                    image: '../img/segnaletica-verticale.png',
                    title: 'Contact',
                }
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="text">
                <h1>Our specialities<span class="oragePoint">.</span></h1>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nam temporibus officia impedit saepe eligendi.</p>
                <div>_________</div>
            </div>
            <div class="cards">
                <div class="card" v-for="card in cards">
                    <img :src="card.image" :alt="card.title">
                    <h3>{{ card.title }}</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio quam perspiciatis exercitationem sint non tempore quidem.</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    section {
        position: absolute;
        left: 0;
        right: 0;
        top: 810px;
        .container {
            max-width: 1760px;
            padding: 30px;
            margin: auto;
            background-color: white;
            .text {
                text-align: center;
                padding-bottom: 30px;
                p {
                    padding: 10px 0;
                }
                div {
                    color: #ff4c19;
                }
            }
            .cards {
                display: flex;
                .card {
                    width: 25%;
                    text-align: center;
                    img {
                        width: 150px;
                        height: 150px;
                        color: #ff4c19;
                    }
                }
            }
        }
    }
</style>