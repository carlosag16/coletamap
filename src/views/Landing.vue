<template>
  <div class="wrapper">
    <parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout">
          <div
            class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100"
          >
            <h1 class="title" >ColetaMap</h1>
            <h4>
              Seu site de informações de lixo reciclável
            </h4>
            <br />
            <md-button href="#/Localidades" class="md-success md-round" target="_blank">Locais de descarte</md-button>
          </div>
        </div>
      </div>
    </parallax>
    <div class="main main-raised">
      <div class="section">
        <div class="container">
          <div class="md-layout">
            <div
              class="md-layout-item md-size-66 md-xsmall-size-100 mx-auto text-center"
            >
              <h2 class="title text-center">Lixo joga no lugar certo!</h2>
              <h5 class="description">
                hgongeogneln egne ge ewgem geige weiujgwjgwklg 09ugw gwig g  gwopkjglwmgw w gwjfw fwfwif wfw fowf wf wfw fwf wf w9f wfow f0w-f wf wfow
                wjpiwmglçwg wgwgw gwig wgw gwgjw gw9ug wg wgwg wg wgw gwg 
                 w0gjwp gw gw9g wg wgiw giwg nw fw9fguw fwjfiwjfpwf
                 wfwfwfiwf-wkfwf
              </h5>
            </div>
          </div>
          <div class="features text-center">
            <div class="md-layout">
              <div class="md-layout-item md-medium-size-33 md-small-size-100">
                <div class="info">
                  <div class="icon icon-info">
                    <md-icon>recycling</md-icon>
                  </div>
                  <h4 class="info-title">Cuide do lixo</h4>
                  <p>
                    Para o descarte correto do lixo, lembre-se de lavar as embalagens antes de separá-la, 
                    caso não seja possível limpar e tenha resto de material orgânico, 
                    escolha a lixeira para o descarte orgânico.
                  </p>
                </div>
              </div>
              <div class="md-layout-item md-medium-size-33 md-small-size-100">
                <div class="info">
                  <div class="icon icon-success">
                    <md-icon>verified_user</md-icon>
                  </div>
                  <h4 class="info-title">Separação</h4>
                  <p>
                   Para o <span :class="vermelho">plástico</span> utilizamos a cor vermelha,
                   para o <span :class="azul">papel</span> a lixeira é azul,
                   <span :class="amarelo">metal</span> a cor usada é amarelo,
                   <span :class="verde">verde</span> jogamos o lixo na lixiera verde e 
                   por fim <span :class="marrom">marrom</span> para material orgânico.
                  </p>
                </div>
                <br>
                <img :src="lixeira"
                /> 
              </div>
              <div class="md-layout-item md-medium-size-33 md-small-size-100">
                <div class="info">
                  <div class="icon icon-danger">
                    <md-icon>map</md-icon>
                  </div>
                  <h4 class="info-title">Local correto de descarte</h4>
                  <p>
                    Atráves da nossa plataforma, saiba qual o local correto para descartar seu lixo.
                    Saíba o local mais próximo de você com o nosso mapa <a href="#/Localidades">clicando aqui.</a>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  bodyClass: "landing-page",
  props: {
    header: {
      type: String,
      default: require("@/assets/img/bg7.jpg")
    },
    teamImg1: {
      type: String,
      default: require("@/assets/img/faces/avatar.jpg")
    },
    teamImg2: {
      type: String,
      default: require("@/assets/img/faces/christian.jpg")
    },
    teamImg3: {
      type: String,
      default: require("@/assets/img/faces/kendall.jpg")
    },
    lixeira:{
      type: String,
      default: require("@/assets/img/lixeiras.jpg")
    }
  },
  data() {
    return {
      name: null,
      email: null,
      message: null,
      estaAtivo: true,
      vermelho: "vermelho",
      azul: "azul",
      amarelo: "amarelo",
      verde: "verde",
      marrom:"marrom"
    };
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
    }
  }
}
</script>

<style lang="scss" scoped>
.md-card-actions.text-center {
  display: flex;
  justify-content: center !important;
}
.contact-form {
  margin-top: 30px;
}

.md-has-textarea + .md-layout {
  margin-top: 15px;
}

.md-round {
  color: red;
  background-color: red;
}
.titlecolor{
  color: red;
}
.vermelho{
  color: red;
}
.azul{
  color: blue;
}
.amarelo{
  color: rgb(119, 119, 4);
}
.verde{
  color: green;
}
.marrom{
  color: brown;
}



</style>
