<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/projects">Projects</router-link> |
    <router-link to="/contact">Contact</router-link>
  </nav>
  <router-view/>
</template>

<style>
/* Add some basic styling for the navigation */
nav {
  padding: 1rem;
  background-color: #f5f5f5;
}

nav a {
  margin: 0 1rem;
  text-decoration: none;
  color: #333;
}

nav a:hover {
  text-decoration: underline;
}
</style>
