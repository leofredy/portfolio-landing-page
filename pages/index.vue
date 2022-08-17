<template>
  <div class="portfolio">
    <main>
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
              <img width="198" height="184.55" src="~/assets/img/foto-perfil.png" alt="Leonardo de frente">
            </div>
            <div class="portfolio-content-infos">
              <p>
                Olá, sou
              </p>
              <h1>
                Leonardo
              </h1>
              <p>
                Desenvolvedor front-end. Nas horas vagas back-end e mobile.
              </p>
              <ul class="portfolio-content-infos-socialNetwork">
                <li>
                  <a href="https://www.instagram.com/leo.freedy/" target="_blank">
                    <img width="32" height="32" src="~/assets/img/icons/instagram.png" alt="Instagram do Leonardo Freedy">
                  </a>
                </li>
                <li>
                  <a href="https://github.com/leofredy" target="_blank">
                    <img width="32" height="32" src="~/assets/img/icons/github.png" alt="Github do Leonardo Freedy">
                  </a>
                </li>
                <li>
                  <a href="https://www.linkedin.com/in/leonardo-frederico-80282a222/" target="_blank">
                    <img width="32" height="32" src="~/assets/img/icons/icone-linkedin.svg" alt="Discord do Leonardo Freedy">
                  </a>
                </li>
                <li>
                  <a href="https://web.whatsapp.com/send?phone=5518997313158" target="_blank">
                    <img width="32" height="32" src="~/assets/img/icons/whatsapp.png" alt="WhatsApp do Leonardo Freedy">
                  </a>
                </li>
              </ul>
            </div>
          </div>
          <div class="portfolio-shadow portfolio-shadowBottom">
            <img src="~/assets/img/white-shadow.png" alt="">
          </div>
          <div class="portfolio-waterMark">
            <div class="portfolio-waterMark-containerImg">
              <img src="~/assets/img/icons/logo-big.svg" alt="">
            </div>
          </div>
        </div>
      </div>
    </main>
    <footer>
      <div class="row">
        <div class="column">
          <p>© 2022 Todos os direitos reservados.</p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style scoped>
.portfolio-waterMark {
  display: none;
}
.portfolio-shadow {
  position: fixed;
  left: 0;
  z-index: -1;
  width: 100%;
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
  min-height: calc(100vh - 34px);
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
  padding: 0 40px;
}
.portfolio-content-photo img {
  margin: 0 auto;
  width: 100%;
  max-width: 350px;
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
  margin: 0 auto 36px;
  max-width: 366px;
}
.portfolio-content-infos-socialNetwork {
  display: flex;
  justify-content: center;
  align-items: center;
}
.portfolio-content-infos-socialNetwork li:not(:last-child) {
  margin-right: 16px;
}
.portfolio-content-infos-socialNetwork li,
.portfolio-content-infos-socialNetwork img {
  width: 100%;
  max-width: 45px;
}
footer {
  padding: 8px 0 12px;
}
footer p {
  text-align: center;
  font-size: 12px;
}
@media (min-width: 1024px) {
  .portfolio-waterMark {
    position: fixed;
    top: 0;
    bottom: 0;
    right: -9%;
    z-index: -1;
    display: flex;
    align-items: center;
  }
  .portfolio-waterMark-containerImg {
    transform: rotate(-45deg);
    width: 35vw;
  }
  .portfolio-waterMark img {
    width: 100%;
  }
  .portfolio-shadowTop {
    display: none;
  }
  .portfolio-content {
    flex-direction: row;
    align-items: center;
  }
  .portfolio-content-brand {
    order: 1;
    margin-left: 60px;
    min-width: 305px;
  }
  .portfolio-content-infos {
    order: -1;
    text-align: left;
    margin-right: 60px;
  }
  .portfolio-content-photo {
    padding: 0;
  }
  .portfolio-content-infos-socialNetwork {
    justify-content: flex-start;
  }
  .portfolio-content-infos p {
    margin-bottom: 24px;
  }
}
</style>
