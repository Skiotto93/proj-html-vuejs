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
                            <a href="#"><h4>{{ link }}</h4></a>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.container {
    max-width: 1760px;
    display: flex;
    justify-content: space-between;
    padding: 40px 0;
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
            }
        }
    }
    
}
</style>
