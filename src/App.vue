<template>
  <div id="app">
    <!--
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    -->
    <div class="nav-bottom">
      <div class="nav-son justify-between">
        <div>
          <vs-avatar>
            <i class="bx bx-home icons-header"></i>
          </vs-avatar>
        </div>
        <div>
          <vs-avatar>
            <i class="bx bx-search icons-header"></i>
          </vs-avatar>
        </div>
        <div>
          <vs-avatar>
            <i class="bx bx-plus icons-header"></i>
          </vs-avatar>
        </div>
        <div>
          <vs-avatar>
            <i class="bx bx-heart icons-header"></i>
          </vs-avatar>
        </div>
        <div>
          <vs-avatar>
            <i class="bx bx-circle icons-header"></i>
          </vs-avatar>
        </div>
      </div>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
* {
  margin: 0%;
  padding: 0%;
}

::-webkit-scrollbar {
  display: none;
}

.nav-son {
  padding: 10px;
}

.nav-bottom {
  background-color: white;
  position: fixed;
  bottom: 0;
  width: 100%;
  z-index: 100;
}
</style>
