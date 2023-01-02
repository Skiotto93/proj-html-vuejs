<script>
import HeaderLinks from './HeaderLinks.vue';

export default {
    name: 'HeaderNavBar',
    components: {
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
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        
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
</template>

<style lang="scss" scoped>
.container {
    max-width: 1760px;
    display: flex;
    justify-content: space-between;
    padding: 30px 0;
    margin: auto;
    position: fixed;
    left: 0;
    right: 0;
    top: 0;
    z-index: 100;
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
</style>