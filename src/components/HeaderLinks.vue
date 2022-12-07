<script>
export default {
    name: 'HeaderLinks',
    props: {
        navBarLink: String,
    }
}
</script>

<template>
    <li>
        <a href="#"><h5>{{ navBarLink }}</h5></a>
        <i class="fa-solid fa-arrow-right-long d-none"></i>
    </li>
</template>

<style lang="scss" scoped>
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
</style>