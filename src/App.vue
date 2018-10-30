<template>
  <div id="app">
    <div id="brand">
      <router-link to="/">Home</router-link> 
    </div>
    <div id="nav">
      <router-link to="/produtos">Produtos</router-link> 
      <router-link to="/contato">Contato</router-link> 
      <router-link to="/about">Sobre</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">
body{
    background: #ebebeb;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  padding: 30px;
  a {
    font-weight: bold;
    color: #2c3e50;
    margin: 15px;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
#brand{
  padding: 30px;
  float: left;
  margin-left: 130px;
  a {
    // font-size: 20px;
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
