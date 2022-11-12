<template>
  <nav>
    <router-link to="/">Главная</router-link> |
    <router-link to="/skills">Навыки</router-link> |
    <router-link to="/resume">Резюме</router-link> |
    <router-link to="/portfolio">Портфолио</router-link> |
    <router-link to="/contacts">Контакты</router-link> |
    <router-link to="/materials">Материалы</router-link> |
    <router-link to="/jspg">JS playground</router-link>
    <hr style=""/>
  </nav>
  
  <router-view/>
</template>

<style lang="scss">

html {
  background-image: url(assets/bg.jpg);
  background-size: 80%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
  margin: 5px;

  a {
    font-weight: bold;
    color: #4c5e70;

    &.router-link-exact-active {
      color: black;
      text-decoration: overline;
    }
  }

  hr {
    border: 1px solid #4c5e70;
    border-bottom-width: 0;
  }

}
</style>
