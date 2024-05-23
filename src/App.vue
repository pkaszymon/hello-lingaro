<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from '@/components/HelloWorld.vue'
</script>

<template>
  <header>
    
    <div class="wrapper">
      <img alt="Vue logo" class="logo" src="https://lingarogroup.com/hubfs/Lingaro_June_2022/Images/logo_lingaro.svg" width="250" height="150" />
    </div>
    <nav>
      <RouterLink to="/">A page that says hello</RouterLink>
      <RouterLink to="/about">Another reason to hire me</RouterLink>
    </nav>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  /* max-height: 100vh; */
  box-shadow: 1px 4px 5px rgba(156, 156, 156, 0.2); /* Add this line */
  width:100%;
  
  padding-bottom:3rem;
  margin-bottom: 3rem;
  
}

.wrapper {
  display: flex;
  direction: ltr;
  /* gap: 10rem; */
  /* margin-top: 2rem; */
  place-content: center;

}

.logo {
  display: block;
  margin: 2rem auto 0;
}

nav {
  width: 100%;
  font-size: 25px;
  text-align: center;
  margin-top: 1rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
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
