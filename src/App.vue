<script setup>
import { RouterLink, RouterView } from 'vue-router'
import 'vfonts/Lato.css'
</script>

<template>

  <header>
      <nav>
        <h1 class="logo">
          KS
        </h1>
        <div class="buttons">
          <RouterLink class="nav_element" to="/"><n-button quaternary size="large">About</n-button></RouterLink>
          <RouterLink class="nav_element" to="/experience"><n-button quaternary size="large">Experience</n-button></RouterLink>
          <RouterLink class="nav_element" to="/projects"><n-button quaternary size="large">Projects</n-button></RouterLink>
          <RouterLink class="nav_element" to="/contact"><n-button quaternary size="large">Contact</n-button></RouterLink>
          <div class="icons">
            <a class="nav_element" target="#" href="https://www.linkedin.com/in/kenaniah-subrahmanyam/"><img class="icon" src="./assets/linkedin.webp"/></a>
            <a class="nav_element" target="#" href="https://github.com/ken3512"><img class="icon" src="./assets/github.png"/></a>
          </div>
        </div>
      </nav>
  </header>

  <RouterView />
</template>

<style>
  .icons{
    padding-top: 4px;
  }

  .icon{
    width: 30px;
  }

  .logo {
    justify-content: left;
    padding-left: 30px;
  }
  
  nav{
    background: rgb(248,241,241);
    display: flex;
    width: 100%;
  }

  .buttons {
    justify-content: right;
    padding: 15px;
    display: flex;
    width: 100%;
  }

  .nav_element
  {
    margin-right: 10px;
    opacity: 1;
    color: black;
    text-decoration: none;
  }
</style>
