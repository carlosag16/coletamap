<template>
    <div class="wrapper">
       <parallax class="section page-header header-filter" :style="headerStyle">
            <div class="container">
                <div class="md-layout">
                    <div class="md-layout-item md-size-50 md-small-size-70 md-xsmall-size-100">
                        <h1 class="title" >ColetaMap</h1>
                        <h4>
                        Seu site de informações de lixo reciclável
                        </h4>
                        <h1 class="title">pq reciclar seu lixo</h1>
                    </div>
                </div>
            </div>
        </parallax>
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