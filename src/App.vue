<script setup>
import { RouterLink, RouterView } from 'vue-router'
import FooterView from './components/FooterView.vue'

</script>

<template>
  <header>
      <nav id="nav">
        <RouterLink id="a" to="/"> <strong>Home</strong> </RouterLink> |
        <RouterLink to="/about"> <strong>Sobre</strong> </RouterLink>
      </nav>
    
  </header>

  <RouterView />
<footer-view/>

</template>

<style>

#nav a {
    color: #ffffff;
    margin: 1px;
    padding: 0.5%;
    transition: 0.5s;
    font-weight: 600;
    font-size: large;
    
}

#nav :hover {
    color: #a5a5a5;

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fdfeff;
  margin-top: 60px;
  margin-bottom: 100px;
}
html{
  background: url("https://cdn.pixabay.com/photo/2020/08/09/14/25/business-5475663_1280.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-blend-mode: difference;
  min-height: 100%;
  opacity: 1;
}

</style>

