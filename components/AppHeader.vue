<template>
  <header class="header">
    <nuxt-link to="/"> <h1 class="title">Dad Jokes</h1> </nuxt-link>
    <ul>
      <li>
        <nuxt-link to="/jokes" class="header-link">Jokes</nuxt-link>
        <nuxt-link to="/about" class="header-link">About</nuxt-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "AppHeader"
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
  color: #000033;
}
.header ul {
  display: flex;
}
.header-link {
  margin: 0.5rem;
}
</style>
