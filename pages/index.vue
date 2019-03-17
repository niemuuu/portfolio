<template>
  <div class="container-top">
    <div class="section-wrapper">
      <hero-section />
      <!-- About me -->
      <section id="about" class="section">
        <h3 class="title">
          About me
        </h3>
        <div class="container">
          <p>工業高校の電気科を卒業後、石油天然ガス開発企業のメンテナンス業に従事、プラントの安定稼働を支える。</p>
          <p>次第にエンジニアという職業に憧れを持ち、独学で開発手法を学びつつ、LPIC（現LinuC）を取得。</p>
          <p>2017年11月にWebエンジニアとして転職、様々なシステム・サービスの開発を行う。</p>
          <br>
          <p>React.js / Redux / Vue.js / Nuxt.js / TypeScript を用いたSPA開発や、<br>Node.js / Golang を用いたバックエンド開発を得意とする。</p>
        </div>
      </section>

      <!-- Accounts -->
      <section id="accounts" class="section">
        <h3 class="title">
          Accounts
        </h3>
        <div class="field has-addons">
          <p class="control">
            <a class="button" href="http://tmkk.hatenablog.com" alt="Blog link">Blog</a>
          </p>
          <p class="control">
            <a class="button" href="https://twitter.com/niemuuu" alt="Twitter link">Twitter</a>
          </p>
          <p class="control">
            <a class="button" href="https://github.com/niemuuu" alt="GitHub link">GitHub</a>
          </p>
          <p class="control">
            <a class="button" href="https://qiita.com/niemuuu" alt="Qiita link">Qiita</a>
          </p>
          <p class="control">
            <a class="button" href="https://www.wantedly.com/users/37956169" alt="Wantedly link">Wantedly</a>
          </p>
          <p class="control">
            <a class="button" href="https://speakerdeck.com/niemuuu" alt="Speaker Deck link">Speaker Deck</a>
          </p>
        </div>
      </section>

      <!-- Contact -->
      <section id="contact" class="section">
        <h3 class="title">
          Contact
        </h3>
        <p>yorori.too[at]gmail.com</p>
      </section>
    </div>
    <footer class="footer">
      <div class="content has-text-right">
        <p>© 2019 niemuuu</p>
      </div>
    </footer>
  </div>
</template>

<script>
import HeroSection from '~/components/HeroSection'

export default {
  components: {
    HeroSection
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

  p {
    color: gray;
  }
}
</style>
