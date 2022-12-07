<script>
export default {
    name: 'ImportantLinks',
    props: {
        footerlink: String,
    }
}
</script>

<template>
    <div class="link">
        <a>{{ footerlink }}</a>
    </div>
</template>

<style lang="scss" scoped>
.link a {
    padding-bottom: 10px;
    cursor: pointer;
}
a:hover {
    color: white;
    filter: brightness(1);
}
</style>