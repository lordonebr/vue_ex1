<template>
     <div class="postItem">
        <img class="image" v-bind:src="imageSrc" />
        <div class="desc">
            <h5>{{title}}</h5>
            <p>{{text}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: "post",
    props: {
        imageSrc: String,
        title: String,
        text: String
    }
};
</script>

<style scoped>
.postItem {
    clear: left;
    margin: 10px;
}

.image {
    height: 250px;
    width: 200px;
    float: left;
}

.desc {
    height: 240px;
    width: 450px;
    padding: 5px;
    margin-left: 220px;
    border-style: solid;
    border-width: 1px;
    position: relative;
    background: white;
}
</style>