<template>
    <div class="listPost">
      <Post v-for="item in articles" v-bind:key="item" v-bind:post="item" />
    </div>
</template>

<script>
import Post from './Post.vue'

export default {
    name: "container",
    components: {
      Post
    },
    props: {
        articles: Array
    }
};
</script>

<style scoped>
.listPost {
    float: left;
  }
</style>