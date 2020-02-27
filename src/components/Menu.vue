<template>
    <nav class="navStyle">
        <a v-for="item in menuItems" v-bind:key="item" class="itemNav" href="#">{{ item }}</a>
    </nav>
</template>

<script>
export default {
    name: "menu",
    props: {
        menuItems: Array
    }
};
</script>

<style scoped>
.navStyle  {
    text-align: center;
    font-size: 20px;
    margin-top: 20px;
    padding: 5px;
    width: 100%;
    float: left;
    background:  green;
}

.itemNav {
    margin: 10px;
    text-decoration: none;
    color: white;
}
</style>