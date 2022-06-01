<template>
  <main class="portfolio">
    <div class="row">
      <div class="column">
        <div class="portfolio-shadow portfolio-shadowTop">
          <img src="~/assets/img/white-shadow.png" alt="">
        </div>
        <div class="portfolio-content">
          <div class="portfolio-content-brand">
            <div class="portfolio-content-brand-logo">
              <img width="40" height="57" src="~/assets/img/logo.svg" alt="Logo Leonardo Freedy">
            </div>
            <span>
              LEO FREEDY DESENVOLVEDOR
            </span>
          </div>
          <div class="portfolio-content-photo">
            <img width="198" height="184.55" src="~/assets/img/foto.png" alt="Leonardo de frente">
          </div>
          <div class="portfolio-content-infos">
            <p>
              Olá, sou
            </p>
            <h1>
              Leonardo
            </h1>
            <p>
              Desenvolvedor front-end. Nas horas vagas 
              estudo back-end e mobile.
            </p>
            <ul class="portfolio-content-infos-socialNetwork">
              <li>
                <a href="" target="_blank">
                  <img width="32" height="32" src="~/assets/img/icons/instagram.png" alt="Instagram do Leonardo Freedy">
                </a>
              </li>
              <li>
                <a href="" target="_blank">
                  <img width="32" height="32" src="~/assets/img/icons/github.png" alt="Github do Leonardo Freedy">
                </a>
              </li>
              <li>
                <a href="" target="_blank">
                  <img width="32" height="32" src="~/assets/img/icons/discord.png" alt="Discord do Leonardo Freedy">
                </a>
              </li>
              <li>
                <a href="" target="_blank">
                  <img width="32" height="32" src="~/assets/img/icons/whatsapp.png" alt="WhatsApp do Leonardo Freedy">
                </a>
              </li>
            </ul>
          </div>
        </div>
        <div class="portfolio-shadow portfolio-shadowBottom">
          <img src="~/assets/img/white-shadow.png" alt="">
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style scoped>
.portfolio-shadow {
  position: absolute;
  z-index: -1;
}
.portfolio-shadowTop {
  transform: rotate(180deg);
}
.portfolio-shadowBottom {
  bottom: 0;
}
.portfolio-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  min-height: 100vh;
}
.portfolio-content-brand {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 36px;
}
.portfolio-content-brand-logo {
  margin-right: 16px;
}
.portfolio-content-photo {
  margin-bottom: 24px;
}
.portfolio-content-photo img {
  margin: 0 auto;
}
.portfolio-content-infos {
  text-align: center;
}
.portfolio-content-infos p:first-child,
.portfolio-content-infos h1 {
  margin-bottom: 10px;
}
.portfolio-content-infos h1 {
  line-height: 1;
}
.portfolio-content-infos p {
  margin-bottom: 36px;
}
.portfolio-content-infos-socialNetwork {
  display: flex;
  justify-content: center;
  align-items: center;
}
.portfolio-content-infos-socialNetwork li:not(:last-child) {
  margin-right: 16px;
}
</style>