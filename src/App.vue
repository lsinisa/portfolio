<template>
  <div id="app">
    <div id="nav">
      <span>SinisaLugonja</span>
      <a><router-link to="/">technologies</router-link></a>
      <a><router-link to="/about">projects</router-link></a>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

img{
  padding: 1% 0 0 0;
}

#nav {
  position: fixed;
  width: 100%;
  padding: 15px;
  z-index: 99;
  background-color: fuchsia;
  span{
    float: left;
    font-weight: bolder;
  }
  a {
    float: initial;
    padding: .3em;
    font-weight: bold;
    color: #0a0a0a;
    &.router-link-exact-active {
      color: #ffffff;
    }
  }
}
</style>
