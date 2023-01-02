<script setup lang="ts">
import ToolCard from "./toolCard.vue";
import SmallToolCard from "./small-toolCard.vue";
import SliderPage from "./slider-page.vue";
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
              <tool-card tool-name="FIGMA"
                         description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                         dist="Free"
                         image-u-r-l="src/assets/svg/icons/icon_FIGMA.svg"
                         :is-selected="false">
              </tool-card>
              <tool-card tool-name="Notion"
                         description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                         dist="Free & Paid"
                         image-u-r-l="src/assets/svg/icons/icon_Notion.svg"
                         :is-selected="false">
              </tool-card>
              <tool-card tool-name="Sketch"
                         description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                         dist="Trial & Paid"
                         image-u-r-l="src/assets/svg/icons/icon_Sketch.svg"
                         :is-selected="true">
              </tool-card>
              <tool-card tool-name="Slack"
                         description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                         dist="Free & Paid"
                         image-u-r-l="src/assets/svg/icons/icon_Slack.svg"
                         :is-selected="false">
              </tool-card>
              <tool-card tool-name="Visual Studio Code"
                         description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                         dist="Free"
                         image-u-r-l="src/assets/svg/icons/icon_vscode.svg"
                         :is-selected="false">
              </tool-card>
              <tool-card tool-name="Invision"
                         description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                         dist="Free & Paid"
                         image-u-r-l="src/assets/svg/icons/icon_Invision.svg"
                         :is-selected="false">
              </tool-card>
            </div>

            <button type="button" class="popular-tools-loadMore">Load More</button>
        </div>
      </div>

      <div class="layout-trusted-brands">
        <div class="trusted-brands-content">
          <img src="/src/assets/svg/redLight.svg" alt="" class="red-light">

          <h3 class="trusted-brands-title">Trusted more than 150+ brand</h3>

          <div class="trusted-brands-images">
            <img src="/src/assets/svg/icons/logos_microsoft.svg" alt="microsoftLogo">
            <img src="/src/assets/svg/icons/logos_google.svg" alt="googleLogo">
            <img src="/src/assets/svg/icons/logos_slack.svg" alt="slackLogo">
            <img src="/src/assets/svg/icons/logos_wordpress.svg" alt="wordpressLogo">
          </div>

        </div>
      </div>

      <div class="layout-newcomers-tools">
        <div class="newcomers-tools-content">

          <article class="newcomers-tools-info">
            <h1>Newcomer Tools</h1>
            <div class="info-text">
              <p>Wow! see the latest update of the most</p>
              <p>recommended tools from reliable designers </p>
              <p>and developers</p>
            </div>
            <button class="info-button">Explore more</button>
          </article>

          <div class="newcomers-tools-cards">
            <div class="top-cards">
              <small-tool-card tool-name="Zeplin"
                               dist="Free & Paid"
                               description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                               image-u-r-l="src/assets/svg/icons/icon-zeplin.svg"
                               :is-selected="false">
              </small-tool-card>
              <small-tool-card tool-name="PHPStorm"
                               dist="Free"
                               description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                               image-u-r-l="src/assets/svg/icons/icon-phpstorm.svg"
                               :is-selected="true">
              </small-tool-card>
            </div>
            <div class="bot-cards">
              <small-tool-card tool-name="Toolbox"
                               dist="Free"
                               description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                               image-u-r-l="src/assets/svg/icons/icon-toolbox.svg"
                               :is-selected="false">
              </small-tool-card>
              <small-tool-card tool-name="Procreate"
                               dist="Paid"
                               description="Lorem ipsum dolor sit amet, consectetur adipiscing elit."
                               image-u-r-l="src/assets/svg/icons/icon-procreate.svg"
                               :is-selected="false">
              </small-tool-card>
            </div>
          </div>

        </div>
      </div>

      <div class="layout-stories">
        <img src="src/assets/svg/chevron-left.svg" alt="left-arrow">
        <div class="stories-content">
          <slider-page name="Ronald Richards"
                       profession="Product Manager"
                       image-u-r-l="src/assets/svg/ronaldRichardsImage.svg"
                       story-text="Incididunt cillum do sint sint enim ullamco id deserunt mollit qui
          reprehenderit do. Velit ex tempor cillum ad sint occaecat. Do nulla velit
          labore occaecat do deserunt Lorem magna officia incididunt consectetur amet.
          Sunt consectetur veniam minim ex commodo sint non. Occaecat aute officia excepteur non
          laboris id qui ad."
          class="stories-item">
          </slider-page>
          <div class="stories-page">
            <div class="page-number"></div>
            <div class="page-number selected"></div>
            <div class="page-number"></div>
          </div>

        </div>
        <img src="src/assets/svg/chevron-right.svg" alt="right-arrow">
      </div>

      <div class="layout-join-us">
        <div class="join-us-content">

          <div class="join-us-title">
            <h1>Become a contributor?</h1>
            <p>Join us and get tips & tricks to become a great</p>
            <p>Designer and Developer</p>
          </div>

          <div class="join-us-button-input">
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
            padding: 21px 160px 22px 55px
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
          right: 65px
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
        .search-button:active
          animation: buttonAnim 1s ease
      .preview-socials
        position: absolute
        bottom: 0
    .layout-popular-tools
      display: flex
      flex-direction: column
      padding: 200px 100px 200px 100px
      align-items: center
      .popular-tools-content
        display: flex
        flex-direction: column
        align-items: center
        font-family: $font-style-title
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
          overflow: hidden
          padding-top: 110px
          display: grid
          grid-template-rows: 320px 320px
          grid-auto-flow: column
          grid-gap: 100px 25px
          padding-bottom: 100px
        .popular-tools-loadMore
          color: #FF6E30
          cursor: pointer
          font-family: inherit
          font-size: 20px
          font-weight: normal
          border-radius: 8px
          background: none
          height: 64px
          width: 184px
          border: 1px solid #343B40
        .popular-tools-loadMore:active
          animation: buttonAnim 1s ease
    .layout-trusted-brands
      display: flex
      justify-content: center
      padding-bottom: 200px
      .trusted-brands-content
        position: relative
        display: flex
        flex-direction: column
        align-items: center
        padding: 55px 82px 55px 82px
        background-color: #22292F
        border-radius: 25px
        width: 80%
        .trusted-brands-title
          color: $font-color-main
          font-weight: normal
          padding-bottom: 55px
        .trusted-brands-images
          display: flex
          width: 100%
          justify-content: space-between
        .red-light
          position: absolute
          left: 0
          top: 0
          border-radius: 25px
    .layout-newcomers-tools
      padding: 0 110px 200px 110px
      display: flex
      flex-direction: column
      .newcomers-tools-content
        display: flex
        flex-direction: row
        justify-content: space-between
        .newcomers-tools-cards
          display: flex
          flex-direction: column
          .top-cards
            display: flex
            flex-direction: row
          .bot-cards
            display: flex
            flex-direction: row
      .newcomers-tools-info
        font-family: $font-style-title
        h1
          color: $font-color-main
          font-weight: normal
          font-size: 48px
          line-height: 130%
          padding-bottom: 30px
        .info-text
          padding-bottom: 60px
          p
            color: $font-color-decorator
            font-weight: normal
            font-family: $font-style-title
            line-height: 30px
            font-size: 18px
        .info-button
          height: 58px
          width: 198px
          background-color: $background-color-buttons
          border-radius: 8px
          border: none
          color: #FDF5FF
          font-family: inherit
          font-size: 16px
          font-weight: normal
          cursor: pointer
        .info-button:active
          animation: buttonAnim 1s ease
    .layout-stories
      padding: 0 80px 250px 80px
      display: flex
      .stories-content
        display: flex
        flex-direction: column
        align-items: center
        .stories-item
          padding-bottom: 35px
        .stories-page
          display: flex
          flex-direction: row
          align-items: center
          .page-number
            background-color: #2B3036
            height: 6px
            width: 45px
            margin: 0 18px
            border-radius: 4px
          .selected
            background-color: #FF6E30
            height: 8px
    .layout-join-us
      padding-bottom: 250px
      display: flex
      flex-direction: column
      align-items: center
      .join-us-content
        .join-us-title
          padding-bottom: 100px
          display: flex
          flex-direction: column
          align-items: center
          h1
            padding-bottom: 25px
            font-size: 48px
            font-weight: normal
            font-family: $font-style-title
            line-height: 130%
            color: $font-color-main
          p
            font-family: $font-style-title
            line-height: 30px
            font-weight: normal
            font-size: 18px
            color: $font-color-decorator
        .join-us-button-input
          display: flex
          align-items: center
          position: relative
          font-family: $font-style-attention
          .join-us-input
            color: $font-color-main
            padding: 21px 160px 22px 25px
            border: none
            width: 500px
            border-radius: 15px
            background-color: #283036
            outline: none
          .join-us-input::-webkit-search-decoration,
          .join-us-input::-webkit-search-cancel-button,
          .join-us-input::-webkit-search-results-button,
          .join-us-input::-webkit-search-results-decoration
            display: none
          .join-us-button
            display: flex
            align-items: center
            justify-content: center
            position: absolute
            right: 60px
            height: 48px
            width: 130px
            background-color: $background-color-buttons
            border-radius: 8px
            border: none
            color: #FDF5FF
            font-family: inherit
            font-size: 16px
            font-weight: bold
            cursor: pointer
          .join-us-button:active
            animation: buttonAnim 1s ease
</style>
