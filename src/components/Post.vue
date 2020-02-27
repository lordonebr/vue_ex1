<template>
     <div class="postItem">
        <img class="image" v-bind:src="post.imageSrc" />
        <div class="desc">
            <h5>{{post.title}}</h5>
            <p>{{post.text}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: "post",
    props: {
        post: Object
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