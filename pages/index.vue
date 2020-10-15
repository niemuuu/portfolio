<template>
  <div class="container-top">
    <div class="section-wrapper">
      <hero-section />
      <about-section />
      <accounts-section />
      <contact-section />
    </div>
    <footer class="footer">
      <div class="content has-text-centered">
        <p>© 2020 plant</p>
      </div>
    </footer>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'
import AboutSection from '~/components/AboutSection'
import AccountsSection from '~/components/AccountsSection'
import ContactSection from '~/components/ContactSection'

export default {
  components: {
    HeroSection,
    AboutSection,
    AccountsSection,
    ContactSection
  },
  head() {
    return {
      title: 'plant'
    }
  }
}
</script>


<style scoped lang="scss">
.container-top {
  display: flex;
  justify-content: center;
  align-items: center;
  -webkit-flex-direction: column;
  flex-direction: column;

  .section-wrapper {
    max-width: 768px;
  }
}

.title {
  text-align: left;
}

.footer {
  width: 100%;
  padding: 7px 10px;
  background-color: #fff;
}
</style>
