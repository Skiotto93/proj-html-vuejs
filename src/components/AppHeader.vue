<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: ['HOMES', 'PAGES', 'BLOG', 'SHOP', 'EVENTS', 'ELEMENTS']
        }
    }
}

</script>

<template>
    <header>
        <div class="container">
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
    </header>
</template>

<style lang="scss" scoped>
header {
    background-image: url('../img/rev-slider-main-home-img-03.jpg');
    background-position: center;
    background-size: cover;
    height: 890px;
    .container {
    max-width: 1760px;
    display: flex;
    justify-content: space-between;
    padding: 30px 0;
    margin: auto;
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
}

</style>
