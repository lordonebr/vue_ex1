<template>
    <div>
        <div class="logoDiv">
            <h1 class="logoText">{{ title }}</h1>
        </div>
        <div class="mainMenu">
            <ul class="listMenu">
                <li v-for="item in topics" v-bind:key="item" class="listItemMenu">
                    <a class="listItemLink" href="#">{{ item }}</a>
                </li>
            </ul>
            <input class="searchInput" placeholder="Search..." type="text" name="search" />
        </div>
    </div>
</template>

<script>
export default {
    name: "topics",
    props: {
        title: String,
        topics: Array
    }/*,
    data() {
        return {
            topics: [
                {topic: "Topic 1"},
                {topic: "Topic 2"},
                {topic: "Topic 3"},
                {topic: "Topic 4"}
            ]
        };
    }*/
};
</script>

<style scoped>
.logoDiv {
  min-width: 100px;
  display: inline-block;
}
.logoText {
  margin-left: 20px;
  margin-right: 20px;
  padding: 10px;
  background: black;
  color: yellow;
}
.mainMenu {
  float: right;
  margin-top: 10px;
  margin-right: 10px;
}
.listMenu {
  border: 3px solid black;
  border-radius: 8px;
  padding: 5px 20px 5px;
}
.listItemMenu {
  display: inline;
  margin: 0px 10px;
}
.listItemLink {
  text-decoration: none;
  color: black;
}
.searchInput {
  margin-bottom: 10px;
  float: right;
}
</style>
