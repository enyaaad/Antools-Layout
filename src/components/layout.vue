<script setup lang="ts">
import ToolCard from "./toolCard.vue";
</script>

<template>
  <main class="layout">
    <div class="layout-content">

      <div class="layout-preview">
        <section class="preview-content">

          <section class="preview-title">
            <div class="title-upper">
              <h1>Awesome tools for</h1>
              <h1>Designer & Developer<span class="title-dot">.</span></h1>
            </div>
            <div class="title-lower">
              <h3>Antool is a web collection of information on paid or </h3>
              <h3>free Design and Development tools</h3>
            </div>
          </section>

          <div class="preview-input">
            <input type="search" class="search-input" placeholder="find more than 430+ tools...">
            <img src="../assets/svg/icons/search.svg" alt="" class="search-logo">
            <button type="button" class="search-button">Search</button>
          </div>

          <div class="preview-socials">
            <a href=""><img src="../assets/svg/icons/facebooklogo.svg" alt="facebookLogo"></a>
            <a href=""><img src="../assets/svg/icons/instlogo.svg" alt="instagramLogo"></a>
            <a href=""><img src="../assets/svg/icons/twitterlogo.svg" alt="twitterLogo"></a>
          </div>
        </section>
        <img src="../assets/svg/Illustration.svg" alt="preview-backImage" class="preview-back-image">
      </div>

      <div class="layout-popular-tools">
        <div class="popular-tools-content">

            <section class="popular-tools-title">
              <h1>Most Popular Tools</h1>
              <article class="title-text">
                <p>Tools for the best Designers and Developers</p>
                <p>most popularity used in the world</p>
              </article>
            </section>

            <div class="popular-tools-cards">
              <tool-card tool-name="FIGMA" description="Lorem ipsum dolor sit amet, consectetur adipiscing elit." dist="Free" :is-selected="false">
              </tool-card>
              <tool-card tool-name="Sketch" description="Lorem ipsum dolor sit amet, consectetur adipiscing elit." dist="Trial & Paid" :is-selected="false">
              </tool-card>
              <tool-card tool-name="Visual Studio Code" description="Lorem ipsum dolor sit amet, consectetur adipiscing elit." dist="Free" :is-selected="false">
              </tool-card>
              <tool-card tool-name="Notion" description="Lorem ipsum dolor sit amet, consectetur adipiscing elit." dist="Free & Paid" :is-selected="false">
              </tool-card>
              <tool-card tool-name="Slack" description="Lorem ipsum dolor sit amet, consectetur adipiscing elit." dist="Free & Paid" :is-selected="false">
              </tool-card>
              <tool-card tool-name="Invision" description="Lorem ipsum dolor sit amet, consectetur adipiscing elit." dist="Free & Paid" :is-selected="false">
              </tool-card>
            </div>

            <button type="button" class="popular-tools-loadMore">Load More</button>
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
@import "../styles/_variables.sass"

.layout
  width: 100%
  display: flex
  flex-direction: column
  justify-content: center
  .layout-content
    display: flex
    flex-direction: column
    .layout-preview
      max-height: 100vh
      display: flex
      flex-direction: row
      justify-content: space-between
      .preview-content
        padding: 3em 0 0 5em
        display: flex
        flex-direction: column
        position: relative
        .preview-title
          .title-dot
            color: $background-color-buttons
          h1
            font-size: 50px
            line-height: 140%
            color: $font-color-main
            font-weight: normal
          h3
            color: $font-color-decorator
            font-size: 18px
            line-height: 30px
          .title-upper
            margin-bottom: 30px
          .title-lower
            margin-bottom: 60px
        .preview-input
          display: flex
          align-items: center
          position: relative
          font-family: $font-style-attention
          .search-input
            color: $font-color-main
            padding: 21px 55px 22px 55px
            border: none
            width: 500px
            border-radius: 15px
            background-color: #283036
            outline: none
          .search-input::-webkit-search-decoration,
          .search-input::-webkit-search-cancel-button,
          .search-input::-webkit-search-results-button,
          .search-input::-webkit-search-results-decoration
            display: none
        .search-logo
          position: absolute
          padding-left: 18px
        .search-button
          position: absolute
          right: 70px
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
      .preview-socials
        position: absolute
        bottom: 0
    .layout-popular-tools
      display: flex
      flex-direction: column
      padding-top: 200px
      align-items: center
      .popular-tools-content
        .popular-tools-title
          display: flex
          flex-direction: column
          align-items: center
          font-family: $font-style-title
          h1
            font-size: 48px
            color: $font-color-main
            margin-bottom: 25px
            font-weight: normal
          .title-text
            display: flex
            flex-direction: column
            align-items: center
            font-size: 18px
            color: $font-color-decorator
        .popular-tools-cards
          display: grid
          grid-template-rows: 200px 200px
          grid-auto-flow: column
          grid-gap: 5px
          overflow: auto
</style>
