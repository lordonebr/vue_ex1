<template>
  <div id="app">
    <Header title="Teste" v-bind:topics="['Topic 1','Topic 2','Topic 3','Topic 4']" />
    <Menu v-bind:menuItems="['Section 1','Section 2','Section 3','Section 4']" />

    <div class="sideBarDiv">
      <SideBar
        v-bind:items="['Section 1', 'Section 2', 'Section 3', 'Section 4', 'Section 5',
                'Section 6', 'Section 7', 'Section 8', 'Section 9', 'Section 10',
                'Section 11', 'Section 12', 'Section 13', 'Section 14', 'Section 15']" />
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Menu from './components/Menu.vue'
import SideBar from './components/SideBar.vue'

export default {
  name: 'App',
  components: {
    Header,
    Menu,
    SideBar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
.sideBarDiv {
  float: right;
}
</style>
