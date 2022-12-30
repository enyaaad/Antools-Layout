<script setup lang="ts">
import ToolCard from "./toolCard.vue";
</script>

<template>
  <main class="layout">
    <div class="layout-content">

      <div class="layout-preview">
        <section class="preview-content">

          <section class="preview-title">
            <p>Awesome tools for Designer & Developer.</p>
            <p>Antool is a web collection of information on paid or free Design
              and Development tools</p>
          </section>

          <div class="preview-input">
            <input type="search" class="search-input" placeholder="Find more than 430+ tools...">
            <button type="button" class="search-button">Search</button>
          </div>

          <div class="preview-socials">
            <img src="" alt="facebookLogo">
            <img src="" alt="instagramLogo">
            <img src="" alt="twitterLogo">
          </div>

          <img src="" alt="preview-backImage">
        </section>
      </div>

      <div class="layout-popular-tools">
        <div class="popular-tools-content">
            <section class="popular-tools-title">
              <h1>Most Popular Tools</h1>
              <p>Tools for the best Designers and Developers
              most popularity used in the world</p>
            </section>

            <div class="popular-tools-cards">
              <tool-card></tool-card>
              <tool-card></tool-card>
              <tool-card></tool-card>
              <tool-card></tool-card>
              <tool-card></tool-card>
              <tool-card></tool-card>
            </div>

            <button type="button" class="popular-tools-loadMore"></button>
        </div>
      </div>

      <div class="layout-trusted-brands">
        <div class="trusted-brands-content">

          <h3 class="trusted-brands-title">Trused more than 150+ brand</h3>

          <div class="trusted-brands-images">
            <img src="" alt="microsoftLogo">
            <img src="" alt="googleLogo">
            <img src="" alt="slackLogo">
            <img src="" alt="wordpressLogo">
          </div>

        </div>
      </div>

      <div class="layout-newcomers-tools">
        <div class="newcomers-tools-content">

          <article class="newcomers-tools-info">
            <h1>Newcomer Tools</h1>
            <p>Wow! see the latest update of the most recommended tools
            from reliable designers and developers</p>
            <button class="info-button">Explore more</button>
          </article>

          <div class="newcomers-tools-cards">
            <tool-card></tool-card>
            <tool-card></tool-card>
            <tool-card></tool-card>
            <tool-card></tool-card>
          </div>

        </div>
      </div>

      <div class="layout-stories">
        <div class="stories-content">

          <img src="" alt="left-arrow">
          <img src="" alt="right-arrow">

          <div class="stories-person">
            <img src="" alt="person">
            <div class="person-card">
              <h2 class="person-name">Ronald Richards</h2>
              <h4 class="person-job">Product Manager</h4>
            </div>
          </div>

          <div class="stories-text">
            <img src="" alt="mark">
            <p>Incididunt cillum do sint sint enim ullamco id deserunt mollit qui 
              reprehenderit do. Velit ex tempor cillum ad sint occaecat. Do nulla velit 
              labore occaecat do deserunt Lorem magna officia incididunt consectetur amet. 
              Sunt consectetur veniam minim ex commodo sint non. Occaecat aute officia excepteur non 
              laboris id qui ad.</p>
          </div>

          <div class="stories-page">
            <div class="page-one">one</div>
            <div class="page-two">two</div>
            <div class="page-three">three</div>
          </div>

        </div>
      </div>

      <div class="layout-join-us">
        <div class="join-us-content">

          <div class="join-us-title">
            <h1>Become a contributor?</h1>
            <p>Join us and get tips & tricks to become a great</p>
            <p>Designer and Developer</p>
          </div>

          <div class="join-us-button">
            <input type="search" class="join-us-input" placeholder="Enter your email...">
            <button type="button" class="join-us-button">Join Us</button>
          </div>

        </div>
      </div>

    </div>
  </main>
</template>

<style lang="sass" scoped>
layout
  display: flex
  flex-direction: column
  justify-content: center
  padding: 20px

</style>
