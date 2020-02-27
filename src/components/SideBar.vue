<template>
    <ul class="sideBarStyle">
        <li v-for="item in items" v-bind:key="item" class="listSideBarStyle">
            <a class="itemSideBar" href="#">{{item}}</a>
        </li>
    </ul>
</template>

<script>
export default {
    name: "sidebar",
    props: {
        items: Array
    }
};
</script>

<style scoped>
.sideBarStyle {
    padding-right: 30px;
    padding-top: 5px;
    padding-bottom: 5px;
    background: black;
    margin-right: 10px;
}

.listSideBarStyle {
    list-style-type: none;
    margin-bottom: 10px;
}

.itemSideBar {
    text-decoration: none;
    color: yellow;
  }
</style>