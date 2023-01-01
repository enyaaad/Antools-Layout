<script>
export default {
  name: "slider-page",
  props:{
    name: String,
    profession: String,
    storyText: String,
    imageURL: String
  }
}
</script>

<template>
  <div class="slider-page">
    <div class="page-content">
      <div class="page-person">
        <div class="page-images">
          <img :src="imageURL" alt="person" class="person-image">
          <img src="src/assets/svg/ImageCircle.svg" alt="" class="image-base">
          <img src="src/assets/svg/orangeLight.svg" alt="" class="orange-light">
        </div>

        <div class="person-card">
          <div class="card-content">
            <h2 class="person-name">{{name}}</h2>
            <h4 class="person-job">{{profession}}</h4>
          </div>
          <img src="src/assets/svg/blueLight.svg" alt="" class="blue-light">

        </div>
      </div>

      <div class="page-text">
        <img src="/src/assets/svg/icons/quote-icon.svg" class="quoteMark">
        <p>{{storyText}}</p>
      </div>


    </div>
  </div>
</template>



<style lang="sass" scoped>
@import "../styles/_variables.sass"

.slider-page
  padding: 0 50px 0 108px
  position: relative
  display: flex
  .page-content
    display: flex
    position: relative
    .page-text
      padding: 120px 0
      p
        letter-spacing: 2px
        line-height: 30px
        font-family: 'Roboto Light', sans-serif
        color: #CDCFD0
        font-size: 14px
      .quoteMark
        position: absolute
        top: 60px
    .page-person
      position: relative
      .page-images
        .image-base
          position: absolute
          z-index: -5
          left: -20px
        .orange-light
          position: absolute
          bottom: 0
          right: 5px
          z-index: -2
      .person-card
        position: absolute
        right: 25px
        bottom: 50px
        height: 90px
        width: 260px
        border-radius: 8px
        backdrop-filter: blur(50px)
        background-clip: padding-box, border-box
        border: solid 1px
        border-image: linear-gradient(rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0))
        background-origin: border-box
        z-index: 1
        overflow: hidden
        .card-content
          padding: 10px 0 15px 20px
          h2
            color: $font-color-main
            font-family: $font-style-title
            font-weight: normal
            font-size: 26px
          h4
            color: $font-color-decorator
            font-family: $font-style-regular
            font-weight: normal
            font-size: 16px
        .blue-light
          position: absolute
          bottom: 0
          right: 0
          filter: blur(20px)




</style>