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
        </div>

        <div class="person-card">
          <h2 class="person-name">{{name}}</h2>
          <h4 class="person-job">{{profession}}</h4>
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
  padding: 0 108px 0 108px
  position: relative
  display: flex
  .page-content
    display: flex
    position: relative
    .page-text
      padding: 120px 0
      p
        letter-spacing: 2px
        font-family: 'Roboto Light', sans-serif
        color: #CDCFD0
      .quoteMark
        position: absolute
        top: 60px
    .page-person
      position: relative
      .page-images
        .image-base
          position: absolute
          z-index: -5
          left: 0
      .person-card
        position: absolute
        border: 1px solid gra

</style>