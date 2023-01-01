<script>
export default {
  name: "small-toolCard",
  props:{
    toolName: String,
    imageURL: String,
    dist: String,
    description: String,
    isSelected: Boolean
  },
}
</script>

<template>
  <div class="tool-card" v-if="!isSelected">
    <div class="tool-card-content">
      <div class="card-top">

        <img :src="imageURL" alt="">

        <div class="tool-dist-name">

          <h1>{{toolName}}</h1>
          <h3>{{dist}}</h3>

        </div>
      </div>

      <div class="card-bottom">
        <h4>{{description}}</h4>
      </div>

      <div class="card-lower-icons">
        <div class="icons">
          <img src="/src/assets/svg/icons/icon-like.svg" alt="">
          <img src="/src/assets/svg/icons/icon-folder-innactive.svg" alt="">
        </div>
        <button type="button" class="card-lower-button-innactive">Visit</button>
      </div>
    </div>
  </div>

  <div class="tool-card selected-card" v-else>
    <div class="tool-card-content">
      <img src="/src/assets/svg/orangeLight.svg" alt="" class="orange-light">
      <div class="card-top">

        <img :src="imageURL" alt="">

        <div class="tool-dist-name selected">

          <h1>{{toolName}}</h1>
          <h3>{{dist}}</h3>

        </div>
      </div>

      <div class="card-bottom selected">
        <h4>{{description}}</h4>
      </div>

      <div class="card-lower-icons">
        <div class="icons">
          <img src="/src/assets/svg/icons/flat-color-icons_like.svg" alt="">
          <img src="/src/assets/svg/icons/icon-folder-active.svg" alt="">
        </div>
        <button type="button" class="card-lower-button">Visit</button>
      </div>

    </div>
  </div>
</template>


<style lang="sass" scoped>
@import "../styles/_variables.sass"
.tool-card
  width: 290px
  border-radius: 15px
  border: none
  .tool-card-content
    padding: 33px
    .card-top
      display: flex
      flex-direction: row
      align-items: flex-start
      .tool-dist-name
        margin-left: 30px
        margin-bottom: 30px
        h1
          font-size: 24px
          color: $font-color-main
          font-weight: normal
        h3
          color: $font-color-unselected-card-cost
    .card-bottom
      h4
        font-weight: normal
        font-size: 16px
        font-family: $font-style-regular
        line-height: 30px
        color: $font-color-unselected-card-text
    .card-lower-icons
      display: flex
      align-items: center
      justify-content: space-between
      font-family: $font-style-attention
      .icons
        display: flex
        flex-direction: row
        align-items: stretch
      .card-lower-button
        align-items: end
        height: 42px
        width: 106px
        background-color: $background-color-buttons
        border-radius: 8px
        border: none
        color: #FDF5FF
        font-family: inherit
        font-size: 16px
        font-weight: bold
        cursor: pointer
      .card-lower-button:active
        animation: buttonAnim 1s ease
      .card-lower-button-innactive
        font-family: inherit
        font-size: 16px
        font-weight: bold
        cursor: pointer
        border: none
        background: none
        color: $font-color-decorator
      .card-lower-button-innactive:active
        animation: buttonAnim 1s ease
.selected-card
  background-color: $background-color-selected-cards
  position: relative
  bottom: 20px
.tool-card
  overflow: hidden
  .tool-card-content
    .card-top
      .selected
        z-index: 1
        h1
          color: #E9EAEA
        h3
          color: $font-color-selected-card-cost
    .card-bottom
      padding-bottom: 30px
    .selected
      h4
        color: $font-color-selected-card-text
    .orange-light
      filter: blur(25px)
      z-index: 0
      position: absolute
      top: -100px
      right: -100px


</style>