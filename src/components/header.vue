<script lang="ts">
export default {
  name: "headerComponent"
}
</script>


<template>
  <header class="header">
    <div class="header-content">
      <div class="header-logo">
        <img src="/src/assets/svg/logo.svg" alt="">
        <h1>antools.</h1>
      </div>

      <nav class="header-nav">
        <a href="">Home</a>
        <a href="">Categories</a>
        <a href="">My Collections</a>
        <a href="">Blog</a>
      </nav>

      <div class="header-buttons">
        <button type="button" class="loginButton">Login</button>
        <button type="button" class="registerButton">Sign Up</button>
      </div>

    </div>
  </header>
</template>


<style lang="sass" scoped>
header
  padding: 1.5em 5em
  .header-content
    display: flex
    flex-direction: row
    justify-content: space-between
    .header-logo
      display: flex
      h1
        padding-left: 12px
  .header-nav
    display: flex
    flex-direction: row
    justify-content: space-evenly
    width: 40%
    a
      text-decoration: none

</style>