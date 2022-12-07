<script>
import AppHeaderSon from './AppHeaderSon.vue';
import HeaderLinks from './HeaderLinks.vue';

export default {
    name: 'AppHeader',
    components: {
        AppHeaderSon,
        HeaderLinks,
    },
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
            description: {
                title: 'Our Team',
                text: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nihil voluptates fuga hic reprehenderit eos? Doloremque, voluptate ipsum, fuga corporis vero nihil repellat eius voluptas deserunt a magni sapiente amet perferendis.'
            }
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
                        <HeaderLinks 
                        v-for="link in links" 
                        :navBarLink="link" 
                        />
                        <li>
                            <a href="#">
                                <font-awesome-icon icon="fa-solid fa-magnifying-glass" />
                                <i class="fa-solid fa-arrow-right-long d-none"></i>
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <font-awesome-icon icon="fa-solid fa-bars" />
                                <i class="fa-solid fa-arrow-right-long d-none"></i>
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
        <AppHeaderSon :title="description.title" :text="description.text"/>
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
                position: relative;
                a {
                    text-decoration: none;
                    color: #000;
                    cursor: pointer;
                }
                a:hover {
                    color: #ff4c19;
                }
                .d-none {
                    display: none;
                }
                a:hover + .d-none {
                    display: block;
                    color: #ff4c19;
                    position: absolute;
                    left: 15px;
                    bottom: 1px;
                }
                .fa-magnifying-glass:hover + .d-none {
                    display: block;
                    color: #ff4c19;
                    position: absolute;
                    left: 15px;
                    bottom: 1px;
                }
                .fa-bars:hover + .d-none {
                    display: block;
                    color: #ff4c19;
                    position: absolute;
                    left: 15px;
                    bottom: 1px;
                }
            }
        }
    
    }
}

</style>
