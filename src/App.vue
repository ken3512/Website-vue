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
          <!-- <RouterLink class="nav_element" to="/"><n-button quaternary size="large">About</n-button></RouterLink>
          <RouterLink class="nav_element" to="/experience"><n-button quaternary size="large">Experience</n-button></RouterLink>
          <RouterLink class="nav_element" to="/projects"><n-button quaternary size="large">Projects</n-button></RouterLink>
          <RouterLink class="nav_element" to="/contact"><n-button quaternary size="large">Contact</n-button></RouterLink>
          <div class="icons">
            <a class="nav_element" target="#2" href="https://www.linkedin.com/in/kenaniah-subrahmanyam/"><img class="icon" src="./assets/linkedin.webp"/></a>
            <a class="nav_element" target="#1" href="https://github.com/ken3512"><img class="icon" src="./assets/github.png"/></a>
          </div> -->
          <input id="menu-toggle" type="checkbox" />
          <label class='menu-button-container' for="menu-toggle">
          <div class='menu-button'></div>
          </label>
          <ul class="menu">
                <li><RouterLink to="/"><n-button quaternary size="large">About</n-button></RouterLink></li>
                <li><RouterLink  to="/experience"><n-button quaternary size="large">Experience</n-button></RouterLink></li>
                <li><RouterLink to="/projects"><n-button quaternary size="large">Projects</n-button></RouterLink></li>
                <li><RouterLink  to="/contact"><n-button quaternary size="large">Contact</n-button></RouterLink></li>
                <li><div class="icons">
                  <a class="nav_element" target="#2" href="https://www.linkedin.com/in/kenaniah-subrahmanyam/"><img class="icon" src="./assets/linkedin.webp"/></a>
                  <a class="nav_element" target="#1" href="https://github.com/ken3512"><img class="icon" src="./assets/github.png"/></a>
                </div></li>
          </ul>
        </div>
      </nav>
      <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- <section class="top-nav">
    <h1 class="logo">
          KS
        </h1>
    <input id="menu-toggle" type="checkbox" />
    <label class='menu-button-container' for="menu-toggle">
    <div class='menu-button'></div>
  </label>
    <ul class="menu">
          <li><RouterLink class="nav_element" to="/"><n-button quaternary size="large">About</n-button></RouterLink></li>
          <li><RouterLink class="nav_element" to="/experience"><n-button quaternary size="large">Experience</n-button></RouterLink></li>
          <li><RouterLink class="nav_element" to="/projects"><n-button quaternary size="large">Projects</n-button></RouterLink></li>
          <li><RouterLink class="nav_element" to="/contact"><n-button quaternary size="large">Contact</n-button></RouterLink></li>
          <div class="icons">
            <li><a class="nav_element" target="#2" href="https://www.linkedin.com/in/kenaniah-subrahmanyam/"><img class="icon" src="./assets/linkedin.webp"/></a></li>
            <li><a class="nav_element" target="#1" href="https://github.com/ken3512"><img class="icon" src="./assets/github.png"/></a></li>
        </div>
    </ul>
  </section> -->
  </header>




  <RouterView />
</template>

<style lang="scss">
  @import url(https://fonts.googleapis.com/css?family=Raleway);



* {
  font-family: "Raleway";
  box-sizing: border-box;
}

.top-nav {
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  background-color: #00BAF0;
  background: linear-gradient(to left, #f46b45, #eea849);
  /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  color: #FFF;
  height: 50px;
  padding: 1em;
}

.menu {
  display: flex;
  flex-direction: row;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu > li {
  margin: 0 0.1rem;
  overflow: hidden;
}

.menu-button-container {
  display: none;
  height: 100%;
  width: 30px;
  cursor: pointer;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

#menu-toggle {
  display: none;
}

.menu-button,
.menu-button::before,
.menu-button::after {
  display: block;
  background-color: #fff;
  position: absolute;
  height: 4px;
  width: 30px;
  transition: transform 400ms cubic-bezier(0.23, 1, 0.32, 1);
  border-radius: 2px;
}

.menu-button::before {
  content: '';
  margin-top: -8px;
}

.menu-button::after {
  content: '';
  margin-top: 8px;
}

#menu-toggle:checked + .menu-button-container .menu-button::before {
  margin-top: 0px;
  transform: rotate(405deg);
}

#menu-toggle:checked + .menu-button-container .menu-button {
  background: rgba(255, 255, 255, 0);
}

#menu-toggle:checked + .menu-button-container .menu-button::after {
  margin-top: 0px;
  transform: rotate(-405deg);
}

@media (max-width: 700px) {
  .menu-button-container {
    display: flex;
  }
  .menu {
    position: absolute;
    top: 0;
    margin-top: 50px;
    left: 0;
    flex-direction: column;
    width: 100%;
    justify-content: center;
    align-items: center;
  }
  #menu-toggle ~ .menu li {
    height: 0;
    margin: 0;
    padding: 0;
    border: 0;
    transition: height 400ms cubic-bezier(0.23, 1, 0.32, 1);
  }
  #menu-toggle:checked ~ .menu li {
    border: 1px solid #333;
    height: 2.5em;
    padding: 0.5em;
    transition: height 400ms cubic-bezier(0.23, 1, 0.32, 1);
  }
  .menu > li {
    display: flex;
    justify-content: center;
    margin: 0;
    padding: 0.5em 0;
    width: 100%;
    color: white;
    background-color: #222;
  }
  .menu > li:not(:last-child) {
    border-bottom: 1px solid #444;
  }
}

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
