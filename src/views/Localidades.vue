<template>
    <div>
      <parallax class="section page-header header-filter" :style="headerStyle">
        <div class="container">
          <div class="md-layout">
            <div class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100">
              <h1 class="title">Localidades de descarte</h1>
              <h4>
                Seu site de informações de lixo reciclável
              </h4>
              <br />
              <p id="App"><Map/></p>
            </div>
          </div>
        </div>
      </parallax> 
    </div>
</template>

<script>
import Map from '../../src/components/Map';

export default {
  name: 'App',
  components: {
    Map
  },
  computed: {
    headerStyle() {
      return {
        backgroundImage: `url(${this.header})`
      };
    }
  },
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
    }
  },
}

</script>

<style lang="scss" scoped>

</style>
<parallax class="section page-header header-filter" :style="headerStyle">
      <div class="container">
        <div class="md-layout">
          <div
            class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100"
          >
            <h1 class="title">Localidades de descarte</h1>
            <h4>
              Seu site de informações de lixo reciclável
            </h4>
            <br />
            <p id="App">
              <Map/>
            </p>
          </div>
        </div>
      </div>
</parallax>