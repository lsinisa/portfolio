<template>
  <div id="app">
    <div id="nav">
      <span>
        Sinisa<b>Lugonja</b>
      </span>
      <a>
        <router-link to="/">technologies</router-link>
      </a>
      <a>
        <router-link to="/proj">projects</router-link>
      </a>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
* {
  width: 100%;
  background-color: #000;
  border:0 none;
  margin: 0;
  position: relative;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  text-align: center;
  color: #2c3e50;
}
#nav{
  padding: .5em 0 .5em 0;
a {
  padding: .4em .4em;
  margin: auto .5em;
  text-decoration: none;
  color: #fff;
  z-index: 1;
  font-weight: bold;
  &.router-link-exact-active {
    background: #fff;
    border-radius: .3em;
    color: #000;
  }
}
a:before {
  content: "";
  position: absolute;
  width:  100%;
  height: .2em;
  bottom: .1em;
  left: 0;
  background: #fff;
  visibility: hidden;
  transform: scaleX(0);
  transition: .3s ease-in-out;
}
a:hover:before{
  visibility: visible;
  transform: scaleX(.7);
}
}
</style>
