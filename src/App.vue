<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    
    <div class="wrapper">
      <img alt="Vue logo" class="logo" src="https://lingarogroup.com/hubfs/Lingaro_June_2022/Images/logo_lingaro.svg" width="250" height="150" />
    </div>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">Another reason to hire me</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.wrapper {
  display: flex;
  direction: ltr;
  gap: 10rem;
  margin-top: 10rem;
  place-content: center;

}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 25px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
   /* color: var(--color-text); */
  color: #773dbd;
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

</style>
