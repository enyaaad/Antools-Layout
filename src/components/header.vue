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
        <a href="" class="nav-element">Home</a>
        <a href="" class="nav-element">Categories</a>
        <a href="" class="nav-element">My Collections</a>
        <a href="" class="nav-element">Blog</a>
      </nav>

      <div class="header-buttons">
        <button type="button" class="loginButton">Login</button>
        <button type="button" class="registerButton">Sign Up</button>
      </div>

    </div>
  </header>
</template>


<style lang="sass" scoped>
@import "../styles/_variables.sass"
header
  padding: 1.5em 5em
  height: $header-height
  .header-content
    display: flex
    flex-direction: row
    justify-content: space-between
    .header-logo
      display: flex
      align-items: center
      h1
        padding-left: 12px
        color: $font-color-decorator
        font-size: 22px
  .header-nav
    align-items: center
    display: flex
    flex-direction: row
    justify-content: space-evenly
    width: 40%
    a
      font-size: 16px
      font-family: $font-style-title
      text-decoration: none
      color: $font-color-decorator
    .nav-element:active
      animation: buttonAnim 1s ease
  .header-buttons
    display: flex
    align-items: center
    font-family: $font-style-attention
    .loginButton
      margin-right: 40px
      background: none
      color: $font-color-additional
      border: none
      padding: 0
      font-size: 16px
      font-family: inherit
      font-weight: bold
      cursor: pointer
      outline: inherit
    .registerButton
      height: 48px
      width: 118px
      background-color: $background-color-buttons
      border-radius: 8px
      border: none
      color: #FDF5FF
      font-family: inherit
      font-size: 16px
      font-weight: bold
      cursor: pointer
    .registerButton:active
      animation: buttonAnim 1s ease
</style>