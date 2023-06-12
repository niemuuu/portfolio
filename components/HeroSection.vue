<script setup lang="ts">
import { computed, ref } from 'vue'
import { onMounted } from '@vue/runtime-core'

const windowWidth = ref(0)
const updateWindowWidth = () => windowWidth.value = window.innerWidth
const isMobile = computed(() => windowWidth.value <= 768)

onMounted(() => {
  windowWidth.value = window.innerWidth
  window.addEventListener('resize', updateWindowWidth)
})

defineExpose({ windowWidth, isMobile })
</script>

<template>
  <section class="hero is-fullheight is-fullheight-with-navbar">
    <div class="hero-body">
      <div class="container">
        <figure class="image icon">
          <img class="is-rounded" src="~/assets/my_icon.jpg">
        </figure>
        <h1 class="title is-1">
          plant
        </h1>
        <h2 class="subtitle is-4">
          <p v-if="!isMobile">Web Developer | Curious Explorer</p>
          <div v-else>
            <p>Web Developer</p>
            <p>Curious Explorer</p>
          </div>
        </h2>
        <div class="tabs is-centered is-medium">
          <ul>
            <li><a href="#about" alt="about link">About me</a></li>
            <li><a href="#accounts" alt="accounts link">Accounts</a></li>
            <li><a href="#public-works" alt="public-works link">Public Works</a></li>
            <li><a href="#contact" alt="contact link">Contact</a></li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@import "~/node_modules/bulma/sass/utilities/mixins";

.container {
  display: flex;
  -webkit-flex-direction: column;
  flex-direction: column;
  align-items: center;

  .icon {
    width: 16rem;
    height: 16rem;
  }
}

@include mobile {
  .container .icon {
    width: 14rem;
    height: 14rem;
  }

  .tabs ul {
    display: flex;
    flex-direction: column;

    a {
      border: none
    }
  }
}

.title {
  margin-top: 1rem;
  margin-bottom: 2rem;
}
</style>
