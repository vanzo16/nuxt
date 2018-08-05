<template>
  <nav class="navigation">
    <nuxt-link to="/">Home page</nuxt-link>
    <nuxt-link to="about">About page</nuxt-link>
    <nuxt-link to="contact">Contact page</nuxt-link>
  </nav>
</template>


<style>
.navigation {
    font-size: 24px;
    padding: 40px;
    text-align: right;
}
.navigation a {
  padding: 10px;
  color: #fff;
  text-decoration: none;
  text-transform: uppercase;
}
</style>