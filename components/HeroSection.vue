<template>
  <section class="hero is-fullheight is-fullheight-with-navbar">
    <div class="hero-body">
      <div class="container">
        <figure class="image is-128x128">
          <img class="is-rounded" src="~/assets/my_icon.jpg">
        </figure>
        <h1 class="title is-1">
          Toxoxi
        </h1>
        <h2 class="subtitle is-3">
          Web Developer
        </h2>
        <div class="tabs is-centered is-medium">
          <ul>
            <li><a href="#about" alt="about link">About me</a></li>
            <li><a href="#accounts" alt="accounts link">Accounts</a></li>
            <li><a href="#contact" alt="contact link">Contact</a></li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.container {
  display: flex;
  -webkit-flex-direction: column;
  flex-direction: column;
  align-items: center;
}

.title {
  margin-top: 10px;
}
</style>
