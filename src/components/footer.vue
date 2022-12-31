<script>
export default {
  name: "footerComponent"
}
</script>


<template>
  <footer class="footer">
    <div class="footer-content">

      <section class="footer-copyright">

        <div class="footer-logo">
          <img src="/src/assets/svg/logo.svg" alt="">
          <h1>antools.</h1>
        </div>
        <div class="copyright-text">
          <h5>Copyright 2021. Antools.</h5>
          <p>Antool is a web collection of</p>
          <p>information on paid of free Design</p>
          <p>and Development tools</p>
        </div>

      </section>

      <section class="footer-contact-us">
        <h1>Contact Us</h1>
        <p>+621987463</p>
        <p>M Building, No.10 A</p>
        <p>antools@awesome.com</p>
      </section>

      <section class="footer-categories">
        <h1>Categories</h1>
        <p>Design</p>
        <p>Development</p>
      </section>

      <section class="footer-company-info">
        <h1>Company Info</h1>
        <p>About us</p>
        <p>Our Partners</p>
        <p>Blog</p>
      </section>

    </div>
  </footer>
</template>


<style lang="sass" scoped>
@import "../styles/_variables.sass"
footer
  border: 0.5px #40464B solid
  padding: 70px 230px 100px 110px
  .footer-content
    display: flex
    flex-direction: row
    width: 100%
    justify-content: space-between
    .footer-copyright

      .footer-logo
        display: flex
        align-items: center
        padding-bottom: 25px
        h1
          padding-left: 12px
          color: $font-color-main
          font-size: 22px
          font-weight: normal
          align-items: center
      .copyright-text
        h5
          padding-bottom: 21px
          font-family: $font-style-title
          font-size: 16px
          color: $font-color-main
        p
          line-height: 25px
          font-family: $font-style-regular
          color: $font-color-decorator
    .footer-contact-us
      display: flex
      flex-direction: column
      h1
        padding-bottom: 20px
        font-family: $font-style-title
        font-size: 20px
        font-weight: normal
        color: $font-color-main
      p
        font-family: $font-style-title
        padding-bottom: 10px
        color: $font-color-decorator
        font-size: 16px
    .footer-categories
      display: flex
      flex-direction: column
      h1
        padding-bottom: 20px
        font-weight: normal
        font-size: 20px
        font-family: $font-style-title
        color: $font-color-main
      p
        padding-bottom: 10px
        font-size: 16px
        color: $font-color-decorator
        font-family: $font-style-title
    .footer-company-info
      display: flex
      flex-direction: column
      h1
        padding-bottom: 20px
        color: $font-color-main
        font-size: 20px
        font-weight: normal
      p
        font-size: 16px
        padding-bottom: 10px
        color: $font-color-decorator
        font-family: $font-style-title


</style>