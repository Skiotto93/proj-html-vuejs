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
.link {
    padding-bottom: 10px;
    a:hover {
        cursor: pointer;
        color: white;
        filter: brightness(1);
    }
}
</style>