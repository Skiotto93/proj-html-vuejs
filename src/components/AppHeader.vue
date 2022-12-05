<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                'HOMES',
                'PAGES',
                'BLOG',
                'SHOP',
                'EVENTS',
                'ELEMENTS'
                ],
            images: [],

        }
    }
}

</script>

<template>
    <header>
        <div class="container">
            <i class="fa-solid fa-arrow fa-arrow-right-long"></i>
            <i class="fa-solid fa-arrow fa-arrow-left-long"></i>
            <div class="logo">
                <img src="../img/logo-img-01.png" alt="logo">
            </div>
            <div class="nav-header">
                <nav>
                    <ul>
                        <li v-for="link in links">
                            <a href="#"><h5>{{ link }}</h5></a>
                        </li>
                        <li>
                            <a href="#">
                                <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <font-awesome-icon icon="fa-solid fa-bars" />
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
        <div class="text-header">
            <h1>Our Team<span class="oragePoint">.</span></h1>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil voluptates fuga hic reprehenderit eos? Doloremque, voluptate ipsum, fuga corporis vero nihil repellat eius voluptas deserunt a magni sapiente amet perferendis.</p>
            <div class="headerBtn">
                <button type="button" class="button-white">
                    READ MORE
                    <div>
                        <i class="fa-solid fa-arrow-right-long"></i>
                    </div>
                </button>
                <button type="button" class="button-orange">
                    PURCHASE
                    <div>
                        <i class="fa-solid fa-arrow-right-long"></i>
                    </div>
                </button>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
header {
    background-image: url('../img/rev-slider-main-home-img-03.jpg');
    background-position: center;
    background-size: cover;
    height: 890px;
    position: relative;
    .container {
    max-width: 1760px;
    display: flex;
    justify-content: space-between;
    padding: 30px 0;
    margin: auto;
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
        img {
            height: 25px;
        }
        ul {
            display: flex;
            li {
            list-style: none;
            padding: 0 40px;
                a {
                    text-decoration: none;
                    color: #000;
                    cursor: pointer;
                }
                a:hover {
                    color: #ff4c19;
                }
            }
        }
    
    }
    .text-header {
        max-width: 600px;
        position: absolute;
        bottom: 35%;
        right: 55%;
        h1 {
            font-size: 70px;
            span {
                color: #ff4c19;
            }
        }
        .headerBtn {
            padding: 20px 0;
            display: flex;
            
            .button-white {
                padding: 10px;
                background-color: white;
                display: flex;
                border: none;
                cursor: pointer;
                div {
                    margin-left: 20px;
                    padding-left: 10px;
                    border-left: 1px solid;
                    i {
                        width: 30px;                        
                    }
                }
            }
            .button-orange {
                padding: 10px;
                margin-left: 20px;
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
            }
        }
    }
}

</style>
