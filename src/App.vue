<script setup>
import { RouterLink, RouterView } from 'vue-router'
import 'vfonts/Lato.css'
import $ from 'jquery'
</script>

<template>
  <header>
      <nav>
        <h1 class="logo">
          KS
        </h1>
        <div class="buttons">
          <input id="menu-toggle" type="checkbox"/>
          <label class='menu-button-container' for="menu-toggle">
            <div class='menu-button'></div>
          </label>
          <ul class="menu" @:change="updateNav()">
                <li><RouterLink to="/"><n-button quaternary size="large" id="about" @:click="closeNav()">About</n-button></RouterLink></li>
                <li><RouterLink  to="/experience"><n-button quaternary size="large" id="experience" @:click="closeNav()">Experience</n-button></RouterLink></li>
                <li><RouterLink to="/projects"><n-button quaternary size="large" id="projects" @:click="closeNav()">Projects</n-button></RouterLink></li>
                <li><RouterLink  to="/contact"><n-button quaternary size="large" id="contact" @:click="closeNav()">Contact</n-button></RouterLink></li>
                <li class="border"><div class="icons">
                  <a class="nav_element" target="#2" href="https://www.linkedin.com/in/kenaniah-subrahmanyam/"><img class="icon" src="./assets/linkedin.webp"/></a>
                  <a class="nav_element" target="#1" href="https://github.com/ken3512"><img class="icon" src="./assets/github.png"/></a>
                </div></li>
          </ul>
        </div>
      </nav>
      <n-button quaternary size="large" id="temp" @:click="activate()">Contact</n-button>
  </header>
  <RouterView />
</template>


<script>
export default{
  name: 'App',
  data(){
    return{
      
    }
  },
  mounted()
  {
    this.$nextTick(() => {
      window.addEventListener('resize', this.updateNav);
    })
  },
  methods:
  {
    closeNav(){
      document.getElementById("menu-toggle").checked = false;
    },
    activate()
    {
      // document.getElementById("about").disabled = true;
      // $("#about").attr("disabled");
      console.log($("#about").attr("disabled", true));
    },
    updateNav()
    {
      if(window.innerWidth > 509)
      {
        document.getElementById("menu-toggle").checked = false;
      }
    }
  },
}
</script>


<style lang="scss" scoped>
  @import url(https://fonts.googleapis.com/css?family=Raleway);

* {
  box-sizing: border-box;
}

#about{
}

.menu {
  z-index:10;
  position:relative;
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
  background-color: #000000;
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

@media (max-width: 509px) {
  .menu-button-container {
    display: flex;
  }
  .menu {
    position: absolute;
    top: 0;
    margin-top: 68px;
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
    height: 3.5em;
    padding: 0.4em;
    transition: height 400ms cubic-bezier(0.23, 1, 0.32, 1);
  }
  #menu-toggle:checked ~ .menu .border {
    border-bottom: 1px solid #000;
  }
  .menu > li {
    display: flex;
    justify-content: center;
    margin: 0;
    padding: 0.5em 0;
    width: 100%;
    color: white;
    background-color: rgb(248,241,241);
  }
  .menu > li:not(:last-child) {
    border-bottom: 1px solid #444;
  }
}

  .icons{
    padding-top: 4px;
    padding-left: 9px;
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
