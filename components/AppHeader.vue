<template>
  <header class="header">
    <v-app-bar color="indigo darken-4" dark>
      <v-toolbar-title> Dad Jokes </v-toolbar-title>

      <div class="flex-grow-1" />

      <nuxt-link to="/">
        Home
      </nuxt-link>

      <nuxt-link to="/jokes">
        Jokes
      </nuxt-link>

      <nuxt-link to="/about">
        About
      </nuxt-link>
    </v-app-bar>
  </header>
</template>

<script>
export default {
  name: 'AppHeader'
};
</script>

<style>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 1rem;
  padding-bottom: 1rem;
  border-bottom: 1px dotted #ccc;
}

.header .title {
  font-size: 3rem;
  color: #526488;
}

.header ul {
  display: flex;
}

.header a {
  display: inline-block;
  background: transparent;
  color: #fff;
  padding: 0.3rem 1rem;
  margin-right: 0.5rem;
}
</style>
