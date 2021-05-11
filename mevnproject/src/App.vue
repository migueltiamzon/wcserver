<template>
  <div id="app">
    <template>
      <div class = "container">
      <nav class = "navbar navbar-expand-sm bg-dark navbar-dark">
        <ul class = "navbar-nav">
          <li class = "nav-item">
            <router-link to="/" class = "nav-link">Home</router-link>
          </li>
          <li class = "nav-item">
             <router-link to="/create" class = "nav-link">Create</router-link>
          </li>
          <li class = "nav-item">
             <router-link to="/posts" class = "nav-link">Post</router-link>
          </li>
        </ul>
      </nav><br/>
      <transition name="fade">
        <router-view></router-view>
      </transition>
      </div>
    </template>
  </div>
</template>
<script>
export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>