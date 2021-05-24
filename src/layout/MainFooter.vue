<template>
  <footer
    class="footer"
    :class="{ [`footer-${type}`]: type }"
    :data-background-color="backgroundColor"
  >
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="https://www.creative-tim.com">
              Criado por
            </a>
          </li>
          <li>
            <a href="https:///presentation.creative-tim.com">
              Sobre nós
            </a>
          </li>
          <li>
            <a href="https:///blog.creative-tim.com">
              Sites
            </a>
          </li>
          <li>
            <a href="https://www.creative-tim.com/license">
              Licenses 
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, Feito pela equipe de Eng da computação UFPA. 
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>
<style></style>
