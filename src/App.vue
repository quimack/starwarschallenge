<template>
  <div class="bckgr">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view />
  </div>
</template>

<style lang=scss>
@import '@/assets/_variables.scss';

@font-face {
  font-family: "star-jedi-hollow";
  src: url("@/assets/fonts/StarJediHollow.otf") format("opentype");
}

html,
body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: $text-200;
  margin: 0;
  background-color: $bg-100;
  overflow-x: hidden;
}

.bckgr {
  width: 100vw;
  height: 100vh;
  background: center / cover url(@/assets/images/sw-wallpaper.jpg) no-repeat;
}

nav {
  padding: 1em;
  font-family: 'star-jedi-hollow';
  font-size: 1.4em;
}

nav a {
  font-weight: bold;
  color: $primary-300;
}

nav a.router-link-exact-active {
  color: $primary-100;
}
</style>
